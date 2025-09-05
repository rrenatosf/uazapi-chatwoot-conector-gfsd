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

*Pensado para volume e escala:*
✅ Um único setup serve multi instalações e multi accounts
✅ Criação automática de Inbox
✅ Uso do Redis em todos os processos para otimizar desempenho AO MÁXIMO
✅ Extremamente rápida (envio e recebimento de texto em menos de 2000ms!!)

*Interatividade*
✅ Marcação correta de status no Chatwoot "Sent" (usuário sem sinal/rede ← Reloginho); "Delivered" (entregue com sucesso ← Dois checks); "Read" (Lida pelo usuário ← Checks azuis).
✅ Exibe para o usuário "digitando" enquanto o agente digita no Chatwoot 
✅ Resposta enviada pelo Chatwoot marca mensagem corretamente no Whatsapp
✅ Resposta realizada pelo WhatsApp marca mensagem corretamente no Chatwoot
✅ Mensagens apagadas pelo usuário são MARCADAS (não apagadas 🫣) no Chatwoot
✅ Mensagens apagadas no Chatwoot são apagadas para o usuário corretamente
✅ Envio de reações (ao responder com emoji) ou emoji normal (se enviar sem responder)
✅ Recebimento de contatos (Vcard)
✅ Recebimento de localização (e Localização em tempo real)

*Fila interna*
✅ Mensagens enviadas sequencialmente e rapidamente NUNCA chegarão fora de ordem (resolve quase que 100% bugs envolvendo macros longas)
✅ Retry e tratamento de erro: Se o envio da mensagem pelo Chatwoot falhar, mais duas tentativas são realizadas automaticamente para cada mensagem.
✅ Controle de fila: Se uma mensagem falhar, o agente no Chatwoot pode usar comandos para limpar a fila (para não enviar as mensagens seguintes faltando contexto)

*Arquitetura otimizada*
✅ Inbox pode ser renomeado ou ALTERADO a qualquer momento (não é atrelado à instância de forma rígida)
✅ Regra de negócio do Chatwoot seguida com rigor (não duplica linhas de source_id / contat_inboxes na tabela)

*Segurança*
✅ Token da instância não é trafegado como parâmetro na URL