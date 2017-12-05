FROM centos:7
RUN yum install -y python2
RUN yum install -y epel-release
RUN yum install -y python-pip

<<COPY APPLICATION AND CHANGE WORKING DIRECTORY>>
RUN pip install --upgrade pip
RUN pip install --no-cache-dir -r requirements.txt

<<EXPOSE HTTP PORT>>

<<USE ENTRYPOINT AND CMD TO RUN python app.py>>
