FROM python:3.6-bullseye

COPY ./scrapyd.conf /etc/scrapyd/
VOLUME /etc/scrapyd/ /var/lib/scrapyd/
EXPOSE 6800

RUN apt-get update && apt-get install -y build-essential python3-dev

RUN pip3 install scrapyd dateparser scrapy tldextract pymongo python-slugify dateparser requests pycodestyle autopep8 yapf extruct chompjs unidecode



CMD ["scrapyd", "--pidfile="]