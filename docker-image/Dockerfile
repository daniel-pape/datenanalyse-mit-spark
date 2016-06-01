FROM aquila/zeppelin
MAINTAINER Daniel Pape <daniel.pape@codecentric.de>

RUN mkdir /root/data
#ADD http://labrosa.ee.columbia.edu/millionsong/sites/default/files/AdditionalFiles/unique_tracks.txt /root/data
#ADD http://labrosa.ee.columbia.edu/millionsong/sites/default/files/tasteprofile/sid_mismatches.txt /root/data
RUN sudo apt-get update
RUN sudo apt-get install unzip
ADD http://labrosa.ee.columbia.edu/millionsong/sites/default/files/challenge/train_triplets.txt.zip /root/data
RUN unzip /root/data/train_triplets.txt.zip