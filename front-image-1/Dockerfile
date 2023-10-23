# Use uma imagem base Node.js
FROM node:16

# Defina o diretório de trabalho
WORKDIR /app

# Copie os arquivos do aplicativo React
COPY Front-Vibrato/ .

# Instale as dependências
RUN npm install

# Crie uma versão de produção do aplicativo
RUN npm run build

# Exponha a porta do aplicativo React (3000 por padrão)
EXPOSE 80

# Comando para iniciar o servidor da aplicação React
CMD ["npm", "run", "dev"]
