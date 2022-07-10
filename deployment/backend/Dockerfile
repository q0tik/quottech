FROM python:3.9-buster

RUN mkdir app
WORKDIR /app

ENV PATH="${PATH}:/root/.local/bin"
ENV PYTHONPATH=.

RUN pip install --upgrade pip
RUN pip install poetry
RUN poetry install --no-interaction --no-ansi -vvv

COPY services/backend .