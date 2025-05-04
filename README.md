# steam-promo-alert

# 🔔 Steam Promo Alert – Automação com n8n + WhatsApp

Este projeto é uma automação criada com o [n8n](https://n8n.io/) que monitora o preço de um jogo na Steam (neste caso, *Battlefield 4*) e envia automaticamente uma mensagem no WhatsApp quando o valor promocional estiver abaixo de um limite definido.

> 💡 A ideia é mostrar como pequenas automações podem ter grande potencial — seja para uso pessoal, marketing de afiliados ou desenvolvimento de bots inteligentes.


## ⚙️ Tecnologias e Serviços Utilizados

- [n8n](https://n8n.io/) – plataforma de automação low-code
- [API pública da Steam](https://store.steampowered.com/api/appdetails) – para obter informações de jogos e preços
- [CallMeBot WhatsApp API](https://www.callmebot.com/) – envio da mensagem no WhatsApp

---

## 🎯 Objetivo

Enviar uma notificação no WhatsApp **quando o jogo Battlefield 4 estiver custando menos de R$15,00**.

A mensagem enviada contém:
- Nome do jogo
- Preço original
- Preço promocional
- Porcentagem de desconto
- Link direto para o jogo na Steam

---

## 🧠 Lógica do Fluxo

1. **Disparo manual** (ou agendado)
2. Requisição HTTP para a API da Steam (pegando os dados do app ****)
3. Tratamento da resposta com node de código (extração de nome, preço e desconto)
4. Condição: o preço promocional é menor que R$15?
5. Se sim → envia mensagem no WhatsApp com os dados do jogo

---

## 📸 Prints do Projeto

<p align="center">
  <img src="imgs/fluxo-n8n.png" alt="Fluxo no n8n" width="800"/>
</p>

<p align="center">
  <img src="imgs/mensagem-whatsapp.png" alt="Mensagem no WhatsApp" width="300"/>
</p>

---

## 📁 Arquivos

- `flow.json`: exportação do fluxo n8n. Você pode importar diretamente no seu ambiente n8n para testar ou adaptar.

---

## 🚀 Como Usar

1. Crie uma conta no [n8n.io](https://n8n.io/) ou rode localmente
2. Importe o `flow.json` no seu workspace do n8n
3. Configure seu número de WhatsApp e API Key do [CallMeBot](https://www.callmebot.com/)
4. Teste o fluxo manualmente ou agende conforme preferir

---

## 💼 Aplicações futuras

Essa automação é apenas uma ideia inicial. O conceito pode ser expandido para:

- Monitorar múltiplos jogos ou categorias
- Criar bots de ofertas para redes sociais
- Automatizar campanhas com links de afiliados
- Construir alertas para outros sites (Epic, Nuuvem, etc.)

---

## ✨ Demonstração no TikTok e LinkedIn

Estou usando este projeto como uma peça de portfólio para mostrar o poder da automação simples e acessível — com foco em mostrar como o n8n pode ser uma ferramenta poderosa mesmo sem saber programar profundamente.

---

## 📬 Contato

Se quiser conversar, tirar dúvidas ou adaptar esse projeto para algo real:

**LinkedIn:** www.linkedin.com/in/
lisieux-nunes
  
---

## 🧩 Inspiração

> “Automatizar tarefas simples pode ser o primeiro passo para soluções poderosas.”

