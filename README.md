# Claria AI - Agente Conversacional Inteligente para WhatsApp

A **Claria** é um agente de inteligência artificial avançado projetado para transformar o atendimento e a automação de vendas no WhatsApp. Desenvolvida pelo **Trilha Digital**, a plataforma utiliza modelos de linguagem de última geração (LLMs) para oferecer interações humanas, contextuais e focadas em conversão.

## 🚀 Visão Geral Técnica

O projeto foi construído sob a filosofia de **AI-First**, utilizando uma arquitetura escalável que separa a lógica de orquestração de mensagens da camada de inteligência (LLM).

### Principais Funcionalidades:
- **Integração Nativa:** Conexão direta com a **Meta Cloud API** para alta performance e conformidade.
- **Memória Contextual:** Gerenciamento de estado de conversa para retenção de contexto a longo prazo.
- **RAG (Retrieval-Augmented Generation):** Capacidade de consultar bases de conhecimento específicas do cliente para respostas precisas.
- **Processamento de Intenções:** Classificação em tempo real para direcionamento de leads.

## 🛠 Stack Tecnológica

- **Linguagem Principal:** Python 3.11+
- **Orquestração de IA:** LangChain / LangGraph
- **Modelos de Fundação:** Google Vertex AI (Gemini 1.5 Pro / Flash)
- **Framework de API:** FastAPI (assíncrono para alta concorrência)
- **Banco de Dados & Vetores:** PostgreSQL com pgvector (para busca semântica)
- **Infraestrutura:** Google Cloud Platform (GCP)
- **Interface de Mensagens:** Meta Cloud API (WhatsApp Business)

## 🏗 Arquitetura do Sistema

A Claria opera em um fluxo de microsserviços:
1. **Webhook Handler:** Recebe eventos em tempo real da API da Meta.
2. **Orquestrador de Contexto:** Recupera o histórico do usuário no banco de dados.
3. **Inference Engine:** Processa a entrada através do **Gemini via Vertex AI**, utilizando prompts estruturados para garantir o tom de voz da marca.
4. **Action Layer:** Executa funções (tools) se necessário (ex: verificar disponibilidade em agenda).
5. **Response Delivery:** Envia a resposta final formatada para o usuário.

## 📈 Roadmap de Desenvolvimento

- [x] Integração com Meta Cloud API (Live Mode).
- [x] Implementação de suporte multi-agente.
- [ ] Integração com Google Calendar e CRMs via Google Cloud Functions.
- [ ] Dashboard de análise de sentimentos e métricas de conversão.

## 📄 Licença e Propriedade

Este projeto é propriedade intelectual da **Trilha Digital**. O acesso ao código fonte é restrito aos desenvolvedores autorizados e parceiros estratégicos.

---
Desenvolvido com ❤️ pelo Trilha Digital.
