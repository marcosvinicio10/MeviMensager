FROM python:3.11-slim

WORKDIR /app

# Copiar requirements.txt da raiz (não de uma pasta backend)
COPY requirements.txt .

RUN pip install --upgrade pip
RUN pip install -r requirements.txt

# Copiar todos os arquivos da raiz para o container
COPY . .

# Expor a porta que a API usa
EXPOSE 8000

# Comando para iniciar a aplicação
CMD ["uvicorn", "main:app", "--host", "0.0.0.0", "--port", "8000"]