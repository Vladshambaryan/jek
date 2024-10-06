FROM python
RUN git clone https://github.com/eugene-okulik/cool_web_app.git
ENV COOL_PORT 8080
ENV COOL_IP 0.0.0.0
RUN mkdir logs
ENV COOL_LOG logs
RUN mkdir /usr/share/cool-app
RUN echo "This is a page from docker made by python-magic group" > /usr/share/cool-app/cool-text.txt
EXPOSE 8080/tcp
CMD ["python", "cool_web_app/run.py"]


#  docker build -t eokulik/cool_sitenov21 . # sozdat obraz

#   docker run --rm -p 8888:8080 eokulik/cool_sitenov21     # run

#  http://localhost:8888/

#  ================================================

#  docker run -p 8080:8080 -p 50000:50000 --restart=on-failure -v C:\Users\PC\PycharmProjects\sep_23\dockers\jenkins_home:/var/jenkins_home jenkins/jenkins:lts-jdk17

#  http://localhost:8180/