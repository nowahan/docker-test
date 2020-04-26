FROM testdocker456/test:3

WORKDIR /home/seluser/tools/

ADD .env /home/seluser/tools/

EXPOSE 4444
EXPOSE 5900
EXPOSE 2011

ENTRYPOINT bash -c 'sudo chmod 0777 -R /home/seluser/.pm2/logs/ && cd /home/seluser/tools && git reset --hard HEAD && git pull && npm install && npm run prod && /opt/bin/entry_point.sh'