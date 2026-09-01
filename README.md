// O Token fica salvo nas Propriedades do Script (Configurações > Propriedades do script)
const TOKEN = PropertiesService.getScriptProperties().getProperty("TELEGRAM_TOKEN");
const TELEGRAM_API = "https://api.telegram.org/bot" + TOKEN;
