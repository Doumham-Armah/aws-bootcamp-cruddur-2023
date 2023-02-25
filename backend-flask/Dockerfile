# FROM python:3.10-slim-buster

# WORKDIR /backend-flask

# COPY requirements.txt requirements.txt
# RUN pip3 install -r requirements.txt

# COPY . .

# ENV FLASK_ENV=development

# EXPOSE ${PORT}
# CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567"]






# Stage 1: Build the application
FROM python:3.10-slim-buster AS builder

WORKDIR /backend-flask

COPY requirements.txt requirements.txt
RUN pip3 install --user -r requirements.txt

COPY . .

# Stage 2: Copy the application and dependencies
FROM python:3.10-slim-buster AS runner

WORKDIR /backend-flask

COPY --from=builder /root/.local /root/.local
COPY --from=builder /backend-flask .

ENV FLASK_ENV=development
ENV PORT=4567

EXPOSE ${PORT}
CMD [ "python3", "-m" , "flask", "run", "--host=0.0.0.0", "--port=4567"]