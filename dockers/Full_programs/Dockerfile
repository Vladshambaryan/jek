FROM jenkins/jenkins:lts-jdk17
USER root
RUN apt-get update && apt-get install -y python3 python3-pip wget python3-venv
RUN apt-get install -y libgbm-dev libnss3 libasound2 libatk-bridge2.0-0 libcups2 libxcomposite1 libxdamage1 libxrandr2 libgtk-3-0 libpangocairo-1.0-0
RUN wget -q -O - https://dl-ssl.google.com/linux/linux_signing_key.pub | apt-key add -
RUN sh -c 'echo "deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google-chrome.list'
RUN apt-get update && apt-get install -y google-chrome-stable
RUN python3 -m venv /opt/venv
ENV PATH="/opt/venv/bin:$PATH"
RUN pip install --upgrade pip
RUN pip install pytest-playwright
RUN python3 -m playwright install
USER jenkins

#  docker build -t jenkins_full_programs .  # obraz