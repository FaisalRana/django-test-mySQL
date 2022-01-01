FROM python:3.9.1
ENV PYTHONUNBUFFERED 1
RUN mkdir /my_app_dir
WORKDIR /my_app_dir
ADD requirements.txt /my_app_dir/
RUN pip3 install --upgrade pip && pip install -r requirements.txt
ADD . /my_app_dir/

CMD [ "python3", "manage.py", "runserver", "0.0.0.0:8000"]