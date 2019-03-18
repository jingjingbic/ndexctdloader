# Use an official Python runtime as a parent image
FROM continuumio/miniconda3

RUN apt-get update
RUN apt-get install -y build-essential 

RUN mkdir /tmp/ndexctdloader
COPY ./ /tmp/ndexctdloader/
RUN pip install /tmp/ndexctdloader

RUN rm -rf /tmp/ndexctdloader

RUN mkdir /ndexctdloader
WORKDIR /ndexctdloader

CMD /bin/echo "To use run: ndexloadctd.py"
