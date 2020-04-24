FROM testdocket456/test:1

WORKDIR /home/seluser/api-server/

ADD .env /home/seluser/api-server/

EXPOSE 4444
EXPOSE 5900
EXPOSE 2011

ENTRYPOINT bash -c 'sudo chmod 0777 -R /home/seluser/.pm2/logs/ && /home/seluser/api-server/node_modules/pm2/bin/pm2 start /home/seluser/api-server/index.js && /opt/bin/entry_point.sh'