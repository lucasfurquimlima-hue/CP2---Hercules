# CP2---Hercules
🏋️‍♂️ Projeto IronMind AI
Disciplina: Prompt and AI | FIAP 2026

O IronMind AI é um assistente virtual especializado em musculação e nutrição esportiva. Ele foi projetado para atuar como um Personal Trainer digital, oferecendo orientações técnicas sobre biomecânica, protocolos de treinamento e dicas nutricionais com foco em segurança e performance.

Integrantes:

Pedro Ribeiro Lopes — RM: 570083

Lucas Furquim Lima — RM: 568690

Gustavo Torres de Oliveira — RM: 572952

Rafael Laprega Gontijo Magalhães - RM: 561975

Diogo Chiaradia Santos - RM: 570246

Justificativa -

Escolhemos o domínio fitness devido à crescente demanda por informações precisas sobre saúde e bem-estar. No cenário atual, muitas pessoas buscam orientações rápidas sobre exercícios, mas enfrentam o risco de informações genéricas ou perigosas. O IronMind AI resolve isso ao unir a agilidade da IA com um filtro rigoroso de segurança e embasamento científico.

Dataset -

Nosso dataset foi construído manualmente para garantir a qualidade das respostas técnicas. Ele conta com 10 exemplos estruturados de pares pergunta/resposta que cobrem:

Biomecânica: Execução correta de agachamentos e supinos.

Fisiologia: Recuperação muscular e síntese proteica.

Segurança: Identificação de dores articulares e alertas de interrupção de treino.

Metodologias: Explicações sobre técnicas como Rest-Pause e Deload.

System Prompt -

O System Prompt foi desenhado para criar uma persona de autoridade, mas empática.

Decisões de Engenharia de Prompt:

Segurança em Primeiro Lugar: O modelo é instruído a sempre recomendar acompanhamento profissional presencial e a disparar alertas imediatos em caso de menção a dores.

Tom de Voz: Definido como "Amigável, Motivador e Objetivo", utilizando emojis para humanizar a interação.

Parâmetros Técnicos: Configuramos a temperature 0.7 para permitir uma fala natural e motivadora, sem perder a precisão técnica das respostas.

## 🆚 Comparação: Modelo Base vs. Customizado (IronMind AI)

| Pergunta de Teste | Modelo Base (Llama 3.2:1b) | IronMind AI (Customizado) |
| :--- | :--- | :--- |
| **"Sinto dor na lombar no terra."** | Sugestão genérica de repouso e recomendação médica padrão. | **"PARE IMEDIATAMENTE! 🛑 A dor pode ser falta de ativação do core ou má postura. Revise sua técnica com um profissional!"** |
| **"O que é falha concêntrica?"** | Explicação teórica de dicionário sobre contração muscular. | **"É o ponto onde o músculo não consegue mais subir a carga com técnica perfeita! 💪 Essencial para hipertrofia, use com moderação."** |

Desafio Extra: Interface Interativa (C)
Implementamos uma interface gráfica utilizando ipywidgets no Google Colab. Isso permite que o usuário interaja com o IronMind AI através de um painel visual com caixa de texto e botão de envio, simulando a experiência de um aplicativo real de consultoria.

Aprendizados -

Pedro: Aprendi como o ajuste de parâmetros como temperature são decisivos para equilibrar a precisão técnica com uma comunicação mais fluida e natural.

Lucas: Entendi a importância do few-shot learning (exemplos no Modelfile) para fixar o tom de voz do assistente.

Gustavo: Compreendi que a engenharia de prompt é fundamental para criar barreiras de segurança em temas sensíveis como saúde.

Rafael: Foi interessante ver a portabilidade do Ollama e como um Modelfile resume toda a configuração de uma IA complexa.

Diogo: Aprendi a integrar modelos de IA com interfaces gráficas no Colab, tornando a tecnologia mais acessível para o usuário final.
