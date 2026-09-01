# 🧭 Bússola PRO — Mini App Telegram

O **Bússola PRO** é um Mini App (WebApp) para Telegram focado no registro diário de vitalidade, estado físico, hidratação e nutrição dentro do Método Groppo.

## 📱 Tecnologias
- **Frontend:** HTML5, CSS3, JavaScript Nativo e Telegram WebApp API.
- **Backend:** Google Apps Script + Google Sheets API.

## 🛠️ Como Configurar

### 1. Hospedar o Mini App (Frontend)
1. Suba o arquivo `index.html` para o **GitHub Pages** ou **Vercel**.
2. Copie a URL gerada (ex: `https://seuusuario.github.io/bussola-pro`).

### 2. Configurar no Telegram BotFather
1. Abra o [@BotFather](https://t.me/BotFather) no Telegram.
2. Mande o comando `/newapp` ou configure o botão de WebApp no menu do seu Bot.
3. Cole a URL pública do seu `index.html`.

### 3. Backend no Google Apps Script
1. Crie um novo projeto no Google Apps Script.
2. Adicione os arquivos `Code.gs` e `appsscript.json`.
3. Em **Propriedades do Script**, configure:
   - `TELEGRAM_TOKEN`: Token do seu Bot.
   - `SPREADSHEET_ID`: ID da planilha Google onde as respostas serão salvas.
4. Faça o **Deploy** do projeto como App Web (`Qualquer Pessoa`).
5. Execute a função `configurarWebhook()` para conectar o Telegram ao seu script.
