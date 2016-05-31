FROM aquila/zeppelin
MAINTAINER Daniel Pape <daniel.pape@codecentric.de>

RUN mkdir /root/data
ADD http://labrosa.ee.columbia.edu/millionsong/sites/default/files/AdditionalFiles/unique_tracks.txt /root/data
ADD http://labrosa.ee.columbia.edu/millionsong/sites/default/files/tasteprofile/sid_mismatches.txt /root/data
ADD http://labrosa.ee.columbia.edu/millionsong/sites/default/files/challenge/train_triplets.txt.zip /root/data
RUN tar -xvf /root/data/train_triplets.txt.zip