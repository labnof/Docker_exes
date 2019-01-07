FROM ubuntu:16.04
EXPOSE 8000
RUN apt update && apt upgrade && apt install -y python python3-venv git
RUN /bin/bash -c "git clone https://github.com/labnof/my-first-blog.git"
WORKDIR /my-first-blog
RUN python3 -m venv myvenv 
RUN /bin/bash -c " source myvenv/bin/activate \
	&& python -m pip install --upgrade pip \
    && echo 'Django~=2.0.6' > requirements.txt && pip install -r requirements.txt"  
RUN /bin/bash -c " source myvenv/bin/activate && python ./manage.py migrate"
CMD /bin/bash -c " source myvenv/bin/activate && python ./manage.py runserver"
