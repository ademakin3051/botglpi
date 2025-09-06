
🤖 Chatbot de Suporte com n8n, GLPI, IA e WhatsApp  
📌 Visão Geral  

Este projeto é um chatbot inteligente desenvolvido com **n8n**, integrado ao **GLPI (ITSM - Gestão de Chamados)**, à **OpenAI** e ao **WhatsApp via API Evolution**.  

O objetivo é automatizar o atendimento de suporte, permitindo que usuários abram chamados, consultem o andamento e recebam resumos claros gerados por IA — tudo diretamente pelo WhatsApp ou pela interface web.  

🚀 Funcionalidades  

    ✅ Atendimento automatizado – fluxo inicial guiado para abertura de chamados
    ✅ Integração com GLPI – abertura e consulta de tickets via API REST
    ✅ Consulta de status – acompanhar andamento e comentários de chamados
    ✅ Resumo inteligente com IA (GPT-4.1) – organiza informações de forma clara e cronológica
    ✅ Integração com WhatsApp (API Evolution) – usuários podem interagir direto pelo WhatsApp
    ✅ Escalonamento para atendimento humano – quando necessário
    ✅ Feedback em tempo real – respostas claras e dinâmicas

⚙️ Tecnologias Utilizadas  

    n8n → Orquestração dos fluxos de automação
    GLPI API REST → Gestão de chamados (abertura e consulta)
    OpenAI GPT-4.1 → Resumo automático de chamados
    API Evolution (WhatsApp) → Envio e recebimento de mensagens no WhatsApp
    Webhooks → Integração entre serviços
    Variáveis de Ambiente (.env) → Segurança das credenciais e tokens  

🛠️ Arquitetura do Fluxo  

    Usuário inicia atendimento (via web ou WhatsApp)
    O bot apresenta opções:
        Abrir chamado
        Consultar andamento
        Falar com humano
    O n8n coleta informações (nome, e-mail, matrícula, telefone e descrição do problema)
    Integração com GLPI cria ou consulta o chamado via API
    A IA (GPT-4.1) organiza dados de status e comentários em formato amigável
    O usuário recebe resposta no WhatsApp (via API Evolution) ou na interface web
    Se necessário, o bot redireciona para atendimento humano  

🔒 Segurança  

As credenciais e tokens não estão incluídos no repositório.  
Use variáveis de ambiente para configurá-los:  

.env.example  

```

GLPI\_USER\_TOKEN=seu\_token\_aqui
GLPI\_APP\_TOKEN=seu\_app\_token\_aqui
GLPI\_SESSION\_TOKEN=session\_token\_aqui
OPENAI\_API\_KEY=sua\_chave\_openai\_aqui
EVOLUTION\_API\_KEY=sua\_chave\_whatsapp
EVOLUTION\_INSTANCE=seu\_id\_da\_instancia

```

📂 Fluxo n8n  

O repositório inclui o arquivo:  

- **`GLPI_public.json`** → fluxo exportado do n8n que contém:  
  - Webhook para entrada de mensagens  
  - Processamento com IA para interpretar pedidos  
  - Criação e consulta de chamados no GLPI  
  - Resposta estruturada para o usuário via WhatsApp  
  - Escalonamento automático para humano em caso de erro ou solicitação  

📸 Demonstração  

## 🎬 Demonstração em Vídeo Cadastrando Ticket (CHAMADO)  
![Demonstração 1 - Cadastro de Ticket](./TypebotGLPI/demonstração/demonstração1.gif)  

## 🎬 Demonstração em Vídeo Ver Andamento de ticket (CHAMADO)  
![Demonstração 2 - Ver Andamento](./TypebotGLPI/demonstração/demonstração2.gif)  

💡 Diferenciais  

🔹 Integração completa entre chatbot, ITSM (GLPI), IA e WhatsApp  
🔹 Projeto pensado para redução de tempo de resposta e melhora da experiência do usuário  
🔹 Uso de IA generativa para transformar dados técnicos em linguagem clara  
🔹 Estrutura segura e escalável, com uso de variáveis de ambiente  
🔹 Foco em automação corporativa e atendimento multicanal  

## 👨‍💻 Desenvolvido por  

**Natanael Lima**  
*Cyber Security RedTeam | Process Automation RPA*  

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/natanaellima10/) [![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ademakin3051) [![Gmail](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:natanaellima65@gmail.com) [![WhatsApp](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/351925429263)  

---  

🔗 **Links úteis:**  
📧 **Email:** natanaellima65@gmail.com  
🌐 **Blog:** https://www.natanaellima.blog  
```

---
