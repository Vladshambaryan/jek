
FROM jenkins/jenkins:lts-jdk17
USER root
RUN apt-get update && apt-get install -y python3 python3-pip wget python3-venv
RUN wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | apt-key add -
RUN sh -c 'echo "deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google-chrome.list'
RUN apt-get update && apt-get install -y google-chrome-stable
WORKDIR /var/jenkins_home/workspace/API_Test_Project
USER jenkins


#  docker build -t jenkins_api_tests_project .  # obraz

#  docker run -p 8080:8080 -p 50000:50000 --restart=on-failure -v C:\Users\PC\PycharmProjects\sep_23\dockers\jenkins_home:/var/jenkins_home jenkins_playwright_tests

#  http://localhost:8080/

# docker ps ===spicok conteynerov !!!!!!!!!!!!!!!!

# docker stop e26f55494395  conteynera !!!!!!!!!!!!!!!!

# docker rmi -f 7a7add0bf3da принудительное
#=================================================================
#git clone https://github.com/Vladshambaryan/API_Test_Project.git
#pwd
#ls

#cd API_Test_Project
#git pull
#python3 -m venv venv
#. venv/bin/activate
#pip install -r requirements.txt
#pytest -v --alluredir=allure-results

#=================================================================