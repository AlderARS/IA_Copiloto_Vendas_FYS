# 🥤 FYS Copiloto: Gerador de Mensagens e Promos Criativas

Este repositório contém a especificação e os testes do **FYS Copiloto**, um assistente inteligente projetado para gerar textos promocionais, roteiros de vendas e publicações para a **FYS**, marca de refrigerantes do grupo **HEINEKEN**. 

O projeto foi desenvolvido como parte do Desafio de Projeto Final **"Copiloto de Vendas com IA para Atendimento ao Cliente"** na plataforma da [DIO](https://dio.me).

---

## 🎯 O Desafio Escolhido

Em vez de tentar abraçar todas as frentes de vendas, este projeto foca na **Opção C: Geração de Mensagens e Promos Criativas**. 

A FYS se destaca por uma comunicação irreverente, irônica, autodepreciativa e levemente ácida. O desafio deste copiloto é **gerar textos de divulgação que fujam do formato corporativo "perfeito" e robótico**, adaptando-se tanto a contatos B2B (comerciantes e donos de padarias) quanto B2C (consumidor final).

---

## ⚙️ Como o Copiloto Funciona

O comportamento do agente é regido pelas diretrizes documentadas no arquivo [AGENTS.md](AGENTS.md). A IA opera com base nas seguintes entradas fornecidas pelo usuário:

1. **Canal de Comunicação:** WhatsApp, Instagram/Redes Sociais ou Lousa de Giz (PDV).
2. **Público-Alvo:** B2B (Comerciante) ou B2C (Consumidor Final).
3. **Sabor Escolhido:** Guaraná, Limão Siciliano, Laranja, Tônica ou Tônica Zero.
4. **Objetivo/Contexto:** Promoções do tipo "leve 3 pague 2", chegada de estoque, combos locais, etc.

Para cada entrada, o agente gera **duas variações de texto**:
*   **FYS Moderada:** Um texto comercial, seguro e bem-humorado, pronto para uso geral.
*   **FYS Ousada:** Um texto com a acidez máxima da marca, utilizando ironias sobre hábitos de consumo ou sobre a própria concorrência.

---

## 🧠 Diferenciais de Engenharia de Prompt Aplicados

*   **Filtro Jurídico/Marca:** A IA é instruída a nunca citar marcas concorrentes pelo nome real, substituindo-as por referências irônicas (ex: *"aquele refri vermelho de sempre"*).
*   **Identidade Visual Limpa:** Bloqueio total do uso de emojis e hashtags. A IA foca 100% no texto cru, resgatando a comunicação clássica e irônica de cartazes urbanos.
*   **Segmentação por Canal:** O agente aplica regras rígidas de limite de linhas e parágrafos dependendo de onde a mensagem será publicada.

---

## 📁 Estrutura do Repositório

```text
├── AGENTS.md        # Regras de comportamento, tom de voz e instruções do agente.
├── README.md        # Apresentação do projeto e instruções de uso.
└── EXEMPLOS.md      # Exemplos práticos de inputs e saídas geradas pelo modelo.
