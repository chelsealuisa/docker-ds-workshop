# Use a docker image from https://hub.docker.com/_/python/
FROM python:3.8

ENV USERNAME=myuser
ENV UID=1000

RUN useradd -m -s /bin/bash -N -u ${UID} ${USERNAME}
RUN pip install ipython jupyter pandas dash numpy pyarrow

USER ${USERNAME}
WORKDIR /home/${USERNAME}
# COPY connection.json .
COPY app_barplot.py .
COPY app_histogram.py .
COPY data/ ./data/

