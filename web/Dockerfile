FROM node:20

WORKDIR /app

# Copiar package.json do local correto
# Ajuste abaixo para o caminho correto onde estão seus arquivos frontend
COPY /package.json /package-lock.json ./
# ou se estiver na raiz:
# COPY package.json package-lock.json ./

RUN npm install

# Copiar o resto dos arquivos frontend
# Ajuste novamente para o local correto
COPY . .
# ou se estiver na raiz em uma pasta diferente:
# COPY . .

# Expor porta do frontend
EXPOSE 3000

# Comando para iniciar o frontend
CMD ["npm", "start"]