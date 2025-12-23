# 🤖 WhatsApp Chatbot - Assistente Virtual
Este projeto é um chatbot automatizado para WhatsApp desenvolvido em Node.js utilizando a biblioteca whatsapp-web.js. O bot simula um atendimento humano com indicadores de digitação e delays estratégicos, servindo como um primeiro nível de suporte para apresentar planos, tirar dúvidas e encaminhar links de cadastro.

## 📋 Funcionalidades
Login via QR Code: Autenticação segura diretamente pelo terminal.

Detecção de Palavras-chave: Inicia o atendimento ao detectar saudações (Oi, Olá, Menu, Dia, Tarde, Noite).

Menu Interativo: Navegação numérica (Opções 1 a 5).

Simulação Humana:

Utiliza sendStateTyping() para mostrar "Digitando..." no topo da conversa.

Possui funções de delay para não enviar mensagens instantaneamente, tornando a interação mais natural.

Respostas Contextuais: Informações sobre planos, benefícios e links de cadastro.

## 🛠️ Pré-requisitos
Antes de começar, certifique-se de ter instalado em sua máquina:

Node.js (Versão 12 ou superior recomendada)

NPM (Gerenciador de pacotes do Node)

## 🚀 Instalação
Clone este repositório ou baixe o arquivo chatbot.js.

Abra o terminal na pasta do projeto.

Instale as dependências necessárias executando o comando abaixo:

```
npm install whatsapp-web.js qrcode-terminal
```

## ▶️ Como Usar
Execute o script no terminal:

```
node chatbot.js
```

O terminal exibirá um QR Code.

Abra o WhatsApp no seu celular, vá em Aparelhos Conectados > Conectar um aparelho.

Escaneie o QR Code exibido no terminal.

Quando a conexão for estabelecida, a mensagem Tudo certo! WhatsApp conectado. aparecerá.

## ⚙️ Estrutura do Menu
O bot responde às seguintes opções numéricas após a saudação inicial:

1: Como funciona (Explicação do serviço 24h).

2: Valores dos planos (Individual, Família, TOP).

3: Benefícios (Sorteios, receitas, etc).

4: Como aderir (Instruções de adesão).

5: Outras perguntas (Direcionamento para suporte humano).

## 📝 Personalização
Para adaptar o bot ao seu negócio, edite o arquivo chatbot.js:

Links: Substitua https://site.com pelos seus links reais.

Textos: Altere as strings dentro de client.sendMessage para mudar as respostas.

Tempo de Resposta: Ajuste os valores dentro de delay(3000) (onde 3000 = 3 segundos) para tornar o bot mais rápido ou mais lento.

## ⚠️ Aviso Importante
Este projeto utiliza a biblioteca whatsapp-web.js, que não é oficial do WhatsApp. O uso de bots automatizados pode infringir os termos de serviço do WhatsApp, havendo risco de banimento do número.

Recomenda-se utilizar um número de teste ou secundário.

Evite envios em massa (SPAM).

Mantenha os delays (atrasos) para simular comportamento humano e reduzir riscos.

## 📄 Licença
Este projeto é de código aberto e livre para uso educacional e comercial.