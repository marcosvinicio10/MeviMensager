# Dockerfile para o Backend (Django)

# Usar imagem oficial do Python
FROM python:3.11-slim

# Variáveis de ambiente para Django
ENV PYTHONDONTWRITEBYTECODE 1
ENV PYTHONUNBUFFERED 1

# Criar diretório de trabalho
WORKDIR /app

# Instalar dependências
COPY backend/requirements.txt .
RUN pip install --upgrade pip
RUN pip install -r requirements.txt

# Copiar o projeto
COPY Back-End/ .

# Expor a porta padrão do Django
EXPOSE 8000

# Comando para rodar o servidor
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]
