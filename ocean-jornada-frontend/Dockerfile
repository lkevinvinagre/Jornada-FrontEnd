#pull da imagem oficial
FROM node:18-alpine

#definir repositorio de trabalho 
WORKDIR /app

#copiar arquivo de pacotes
COPY package.json .

#instalar modulos do node
RUN npm install

#copiar arquivos
COPY . .

#dar comando para rodar aplicação
CMD [ "npm", "run", "dev" ]
