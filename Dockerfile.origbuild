FROM mono:4.2.1.102

RUN mkdir -p ~/node
RUN chmod 777 ~/node
ADD "./binary/NodeLink.exe" ~/node/
EXPOSE 8090
EXPOSE 2405
CMD [ "mono",  "~/node/NodeLink.exe" ]
