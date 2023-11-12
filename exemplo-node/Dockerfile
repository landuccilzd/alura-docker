#Define qual imagem eu quero puxar
FROM node:14

#Define o diretório ativo dentro da imagem
WORKDIR /app-node

#Define uma variável em tempo de BUILD
ARG PORT=3000

#Define em qual porta a aplicação vai estar exposta
EXPOSE $PORT

#Copia os arquivos locais para /app-node dentro da imagem que estamos criando
COPY . .

#Instala as dependencias do node dentro do /app-node na imagem
RUN npm install

#Inicia o node a partir do /app-node da imagem
ENTRYPOINT npm start