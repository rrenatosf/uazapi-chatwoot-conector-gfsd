# Uazapi Chatwoot Conector - By Years In Box

<div align="center">
  <img src="./.github/assets/Logo Years In Box.png" height="60" alt="Years In Box"/> &nbsp;&nbsp;
  <img src="./.github/assets/Chatwoot Logo.png" height="60" alt="Chatwoot"/> &nbsp;&nbsp;
  <img src="./.github/assets/n8n logo.png" height="60" alt="n8n"/> &nbsp;&nbsp;
  <img src="./.github/assets/Redis Logo.png" height="60" alt="Redis"/> &nbsp;&nbsp;
  <img src="./.github/assets/Uazapi Logo.png" height="60" alt="Uazapi"/> &nbsp;&nbsp;
  <img src="./.github/assets/Whatsapp Logo.png" height="60" alt="WhatsApp"/>
</div>

---

### YIB Conector - Flows do N8N para conectar a Uazapi (API não oficial do Whatsapp) ao Chatwoot

## 🚀 **Pensado para volume e escala:**
- ✅ **Multi-instalações e multi-accounts**: Um único setup serve múltiplas instalações e contas
- ✅ **Criação automática de Inbox**: Setup simplificado e automatizado
- ✅ **Redis em todos os processos**: Otimização máxima de desempenho 
- ✅ **Extremamente rápida**: Envio e recebimento de texto em menos de 1s!!

## 🤝 **Interatividade**
- ✅ **Status de mensagem correto**: 
 - "Sent" (usuário sem sinal/rede ← Relógio)
 - "Delivered" (entregue com sucesso ← Dois checks)  
 - "Read" (lida pelo usuário ← Checks azuis)
- ✅ **Indicador "digitando"**: Exibe para o usuário enquanto agente digita no Chatwoot
- ✅ **Marcação bidirecional**:
 - Resposta enviada pelo Chatwoot marca mensagem corretamente no Whatsapp
 - Resposta realizada pelo WhatsApp marca mensagem corretamente no Chatwoot
- ✅ **Gerenciamento de exclusões**: 
 - Mensagens apagadas pelo usuário são **marcadas** (não apagadas 🫣) no Chatwoot
 - Mensagens apagadas no Chatwoot são removidas corretamente para o usuário
- ✅ **Suporte completo de mídia**:
 - Envio de reações (ao responder com emoji) ou emoji normal (se enviar sem responder)
 - Recebimento de contatos (Vcard)
 - Recebimento de localização (e localização em tempo real)

## ⚡ **Fila interna**
- ✅ **Ordem sequencial garantida**: Mensagens enviadas sequencialmente e rapidamente NUNCA chegarão fora de ordem (resolve quase que 100% **bugs do Chatwoot** envolvendo macros longas)
- ✅ **Sistema de retry e error handler**: Até 3 tentativas automáticas para cada mensagem em caso de falha e com feedback visual para o agente!
- ✅ **Controle de fila**: Se uma mensagem falhar, o agente pode usar comandos para limpar a fila e evitar o envio das mensagens seguintes fora contexto

## 🏗️ **Arquitetura otimizada**
- ✅ **Flexibilidade total**: Inbox pode ser renomeado ou alterado a qualquer momento (não fica atrelado à instância de forma rígida)
- ✅ **Integridade de dados**: Segue rigorosamente regras de negócio do Chatwoot (sem duplicações de source_id na tabela contat_inboxes)

## 🔒 **Segurança**
- ✅ **Token protegido**: Token da instância não é trafegado como parâmetro na URL