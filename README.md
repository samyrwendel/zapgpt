=============== Inicie Copia  

sudo apt update 
sudo apt upgrade -y  
sudo apt install -y nodejs npm 
node -v  
sudo apt install git curl  
sudo apt install gdebi 

wget https://dl.google.com/linux/direct/google-chrome-stable_current_amd64.deb 
sudo gdebi google-chrome-stable_current_amd64.deb 
sudo apt-get -f install  

git clone https://github.com/samyrwendel/zapgpt.git  
cd zapgpt 
mkdir audiobruto 
mkdir audioliquido  

npm install 
npm run install-deps 
npm run install-ffmpeg 
npm install -g 
pm2 --save-dev  

==================== Final Cópia 

nano .env  

# Escrevar a sua chave da Openai: 
OPENAI_API_KEY=ssssssyyyyyysssssllll7777778888899993333 
ctrl + s ; crtl + x  

pm2 start zapgpt.js 
pm2 logs zapgpt 

#### Faça a leitura do qrcode  

# Para voltar ao terminal ctrl + c  
pm2 list  

# Para deletar a instância: 
pm2 delete zapgpt.js  

# Para atualizar: 
git pull 
