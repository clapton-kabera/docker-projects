FROM python:3.9-slim

WORKDIR /app

COPY . .

# I think this is not good layering, this should come before the copying so that it
# does not have to run whenever we modify our flask code
RUN pip install flask

EXPOSE 5000

CMD ["python", "app.py"]
