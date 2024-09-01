# Usa l'immagine base di Node.js
FROM node:14

# Imposta la directory di lavoro
WORKDIR /usr/src/app

# Copia il package.json e package-lock.json
COPY package*.json ./

# Installa le dipendenze
RUN npm install

# Copia il codice sorgente nell'immagine
COPY . .

# Espone la porta su cui l'applicazione ascolterà
EXPOSE 3000

# Comando per avviare l'applicazione
CMD ["node", "app.js"]
