# Dockerfile para o Frontend (React)

# Usar imagem oficial Node.js
FROM node:20

# Criar diretório de trabalho
WORKDIR /app

# Copiar package.json e instalar dependências
COPY web/package.json web/package-lock.json ./
RUN npm install

# Copiar o resto dos arquivos
COPY web/ .

# Expor a porta padrão do React
EXPOSE 3000

# Rodar o app React
CMD ["npm", "start"]
