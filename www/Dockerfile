FROM python
RUN pip install flask
RUN pip install gunicorn
RUN pip install redis
COPY . /src
WORKDIR /src
CMD gunicorn --bind 0.0.0.0:5000 --workers 10 counter:app 
ENV Shridhar=Testing
EXPOSE 5000
