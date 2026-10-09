FROM python:3.8-slim

WORKDIR /app

COPY techtrends/requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY techtrends .

EXPOSE 3111

CMD ["sh", "-c", "python init_db.py && python app.py"]
