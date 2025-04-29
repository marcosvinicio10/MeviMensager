# Dockerfile para o Frontend (React)

# Usar imagem oficial Node.js
FROM node:20

# Criar diretório de trabalho
WORKDIR /app

# Copiar package.json e instalar dependências
COPY frontend/package.json frontend/package-lock.json ./
RUN npm install

# Copiar o resto dos arquivos
COPY frontend/ .

# Expor a porta padrão do React
EXPOSE 3000

# Rodar o app React
CMD ["npm", "start"]
