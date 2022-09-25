FROM python:3.8

COPY techtrends /techtrends
WORKDIR /techtrends
EXPOSE 3111

RUN pip install -r requirements.txt
RUN python init_db.py
# provide a command to run on container start. 
# For example, start the `app.py` application.
CMD [ "python", "app.py" ]