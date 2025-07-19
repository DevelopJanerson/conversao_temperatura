# Etapa 1: imagem base
FROM node:18

# Define o diretório de trabalho no container
WORKDIR /app

# Copia os arquivos de dependências
COPY package*.json ./

# Instala as dependências
RUN npm install

# Copia o restante do código para o container
COPY . .

# Expõe a porta usada pela aplicação
EXPOSE 8080

# Comando para iniciar a aplicação
CMD ["node", "server.js"]
