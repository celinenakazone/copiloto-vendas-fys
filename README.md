🥤 Copiloto de Vendas FYS: Quebra-Gelo
Este repositório contém a especificação e a base de conhecimento de um **Agente de IA Declarativo** projetado para apoiar a força de vendas da **FYS** (marca de refrigerantes do grupo **HEINEKEN**). 
O projeto foi desenvolvido como solução para o Desafio de Projeto **"Copiloto de Vendas com IA para Atendimento ao Cliente"** da DIO.
---
## 🎯 O Desafio de Negócio
Vendedores de rua enfrentam diariamente a barreira da primeira compra (experimentação) e objeções comuns de donos de comércios (como *"meus clientes só pedem a marca líder"* ou *"refrigerante novo não vende"*). Além disso, o tempo do vendedor é escasso para bolar estratégias personalizadas para cada ponto de venda.
---
## 💡 A Solução: Agente Declarativo FYS
Em vez de criar uma aplicação complexa e cheia de telas, este projeto foca na inteligência: a criação de um **Agente de IA especializado**. Utilizando arquivos de configuração comportamental e instruções declarativas, qualquer plataforma compatível com o padrão `AGENTS.md` pode rodar o copiloto de vendas.
O agente recebe:
1. O **tipo de estabelecimento** (ex: bar, padaria, mercadinho).
2. A **objeção do cliente** (ex: "é muito caro", "não conheço a marca").
E gera instantaneamente abordagens de vendas rápidas no tom característico da FYS: leve, bem-humorado, honesto e sem jargões corporativos.
---
## 📂 Arquitetura do Agente
O repositório está organizado da seguinte forma:
* **[AGENTS.md](AGENTS.md):** Define as regras gerais, comportamento e os limites do que a IA pode e não pode sugerir.
* **[agent/persona.md](agent/persona.md):** Detalha a personalidade, tom de voz (sincero e ácido) e fornece exemplos práticos de redação da FYS.
* **[agent/knowledge/brand-fys.md](agent/knowledge/brand-fys.md):** Base de dados da IA contendo informações reais dos produtos, sabores e diferenciais de mercado do grupo Heineken.
* **[skills/break-ice/SKILL.md](skills/break-ice/SKILL.md):** O passo a passo lógico que a IA deve seguir para processar a objeção e gerar as sugestões de roteiro de vendas.
---
## 🛠️ Como Testar o Agente
Você pode testar este agente em qualquer ferramenta de chat de IA (como ChatGPT, Gemini ou Claude). Para isso:
1. Copie o conteúdo dos arquivos `AGENTS.md`, `agent/persona.md` e `agent/knowledge/brand-fys.md` e envie para o chat como instruções iniciais.
2. Em seguida, envie uma objeção real do ponto de venda no formato:
   > *"Estou em uma [Tipo de Estabelecimento] e o dono me disse: [Objeção do Cliente]. Como posso quebrar o gelo?"*
3. A IA responderá com um roteiro presencial rápido e uma mensagem direta para o WhatsApp!
