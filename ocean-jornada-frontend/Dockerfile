#pull da imagem oficial
FROM node:18-alpine

#definir repositorio de trabalho 
WORKDIR /app

#criação da variavel de caminho a armazenar os modulos node
ENV PATH /app/node_modules/.bin:$PATH

#copiar arquivos de pacotes
COPY package.json ./

COPY package-lock.json ./

#instalar modulos do node
RUN npm install

#copiar arquivos
COPY . ./

#dar comando para rodar aplicação
CMD [ "npm", "run", "dev" ]
