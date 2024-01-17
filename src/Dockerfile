# Tipo da aplicação
FROM node:20.11.0

#Pasta final da aplicação
WORKDIR /app

#Para copiar o arquivo package e instalar dependencias novas
COPY package*.json ./

# Instrução para instalar dependenciar da aplicação = package.json
RUN npm install

#Copiar a Aplicação, "." nossa pasta base, "." para pasta base OWRKDIR
COPY . .

# Qual a porta será exposta nossa aplicação
EXPOSE 8080

# Instrução para rodar aplicação
CMD ["node", "server.js"]

#DOCKER BUILD
# docker build -t kube-news -f Dockerfile .

# docker build
# -t kube-news = nome contanaier 
# -f Dockerfile = onde esta arquivo