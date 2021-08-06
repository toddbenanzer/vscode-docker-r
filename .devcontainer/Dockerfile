FROM rocker/r-ver:4.1.0

ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1

RUN apt-get update \
    && apt-get -y install gcc make python3-pip git \
    && rm -rf /var/lib/apt/lists/*s \
    && python3 -m pip --no-cache-dir install radian

RUN install2.r --error \
    rlang \
    jsonlite

CMD [ "/bin/bash" ]