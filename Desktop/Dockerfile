FROM ubuntu

RUN apt-get update && apt-get install git -y 

RUN git clone https://github.com/CristianSch248/ServidorPassagemHttp.git

RUN apt-get update 
RUN apt --assume-yes install openjdk-17-jdk
RUN mkdir /home/serverbus && cd /home/serverbus && git clone https://github.com/CristianSch248/ServidorPassagemHttp.git && cd ServidorPassagemHttp/out/artifacts/trabalhoRafael_jar/
RUN mkdir logs && cd logs && touch log.txt && cd .. 
CMD java -jar /home/serverbus/ServidorPassagemHttp/out/artifacts/trabalhoRafael_jar/trabalhoRafael.jar