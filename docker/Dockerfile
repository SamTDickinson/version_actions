FROM python:3.11.8-slim-bullseye

ENV PIP_DISABLE_PIP_VERSION_CHECK 1
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

WORKDIR /code
COPY . /code

# 3. Install dependencies
RUN pip install -r requirements.txt

CMD ["python3",  "/code/manage.py", "runserver", "0.0.0.0:8000"]

EXPOSE 8000