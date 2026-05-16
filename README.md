# miniguia-estudos-notebooklm
Desafio de projeto da DIO utilizando o NotebookLM para criar um caderno temático e miniguia de estudos sobre Renda Fixa e Renda Variável.
# Miniguia de Estudos: Renda Fixa vs. Renda Variável com NotebookLM

Este repositório foi desenvolvido como parte de um desafio prático de aprendizagem ativa, utilizando a Inteligência Artificial (NotebookLM) como ferramenta de suporte para curadoria, síntese e organização do conhecimento sobre finanças introdutórias.

---

## 1. Contexto e Objetivos de Estudo

O objetivo deste caderno temático é estabelecer uma base sólida sobre os conceitos iniciais do mercado financeiro e de investimentos. O foco principal foi compreender a dinâmica de tomada de decisão para investidores iniciantes, guiando-se pelos seguintes objetivos:
* Compreender a tríade fundamental dos investimentos: **Rentabilidade, Liquidez e Risco**.
* Diferenciar claramente os mecanismos de funcionamento e remuneração da **Renda Fixa** e da **Renda Variável**.
* Identificar os principais ativos iniciais de cada categoria.

---

## 2. Curadoria de Fontes

Para garantir a confiabilidade das respostas e evitar alucinações da IA, o caderno foi alimentado estritamente com materiais oficiais e de acesso aberto de instituições reguladoras do mercado brasileiro:
* **Fonte 1:** *Caderno de Educação Financeira: Gestão de Finanças Pessoais* – Banco Central do Brasil.
* **Fonte 2:** *Guia CVM do Investidor Iniciante* – Comissão de Valores Mobiliários (CVM).
* **Fonte 3:** *Como Funciona o Tesouro Direto* – Secretaria do Tesouro Nacional / B3.

---

## 3. Engenharia de Prompts e "Cicatrizes" (Troubleshooting)

### Estratégia de Prompts Utilizada
Foram desenhados prompts que atribuem papéis específicos à IA (como professor e analista) e delimitam o formato de saída (tabelas e tópicos estruturados), forçando o uso de citações diretas das fontes anexadas.

### Cicatrizes de Testes (O que deu errado e como foi corrigido)
* **Problema encontrado:** No primeiro teste do Prompt 1, a IA gerou um texto excessivamente longo e incluiu conceitos de macroeconomia avançada que não eram o foco do estudo.
* **Solução (Troubleshooting):** O prompt foi refinado adicionando a restrição *"Divida a resposta estritamente nos seguintes tópicos..."* e especificando o uso de *bullet points*. Isso forçou a IA a ser concisa e manter o escopo estritamente focado nos objetivos do repositório.

---

## 4. Miniguia de Estudo (Entrega Final)

### Conjunto de Prompts Reutilizáveis para Revisão

* **Prompt 1 (Resumo Estruturado):** *"Atue como um professor de finanças focado em didática para iniciantes. Com base exclusivamente nas fontes fornecidas, faça um resumo estruturado comparando Renda Fixa e Renda Variável. Divida a resposta estritamente nos seguintes tópicos: 1) Conceito Principal de cada uma, 2) Nível de Risco Atrelado e 3) Exemplos de Ativos citados nos textos. Use bullet points."*
* **Prompt 2 (Glossário de Termos):** *"Analise os documentos inseridos e identifique os 5 principais termos técnicos ou siglas financeiras essenciais para um iniciante (ex: SELIC, CDB, IPCA, Ações, Liquidez). Monte um glossário no formato de tabela contendo: Termo/Sigla | O que significa (segundo as fontes) | Por que é importante saber."*
* **Prompt 3 (Questionário de Autoavaliação):** *"Com base no conteúdo das fontes textuais, crie 3 perguntas de múltipla escolha para testar meus conhecimentos sobre o trade-off entre risco e retorno. Abaixo das perguntas, forneça o gabarito justificando a resposta correta com citações diretas das fontes."*

---

### Resumos Estruturados do Assunto (Resultado do Prompt 1)

* **1) Conceito Principal:**
  * **Renda Fixa:** São investimentos que pagam uma remuneração correspondente a uma taxa de juros em períodos definidos. A regra de remuneração é estipulada no momento da aplicação, podendo ser prefixada ou pós-fixada (atrelada a um indexador de mercado).
  * **Renda Variável:** São investimentos em que o retorno financeiro não pode ser dimensionado ou garantido no momento da aplicação. O ganho futuro dependerá diretamente das oscilações do mercado e do desempenho do ativo.
* **2) Nível de Risco Atrelado:**
  * **Renda Fixa:** Modalidade com menor nível de risco. O principal risco envolvido é o de crédito (possibilidade de a instituição emissora não cumprir com o pagamento).
  * **Renda Variável:** Envolve níveis de risco significativamente maiores. O investidor está exposto ao risco de mercado (volatilidade e oscilações diárias de preços), o que pode resultar tanto em grandes ganhos quanto em perdas de capital.
* **3) Exemplos de Ativos Citados:**
  * **Renda Fixa:** Caderneta de poupança, Títulos Públicos (Tesouro Direto), CDBs, LCIs, LCAs, Debêntures.
  * **Renda Variável:** Ações negociadas na bolsa de valores, Fundos Imobiliários (FIIs) e Fundos de Índices (ETFs).

---

### Glossário de Conceitos Aprendidos (Resultado do Prompt 2)

| Termo / Sigla | O que significa (segundo as fontes) | Por que é importante saber |
| :--- | :--- | :--- |
| **Liquidez** | Capacidade de um ativo ou investimento ser transformado em dinheiro a qualquer momento e por um preço justo. | Ajuda a definir onde colocar o dinheiro com base no prazo dos objetivos (curto, médio ou longo prazo). |
| **Juros Compostos** | Processo em que os juros de cada período são incorporados ao capital principal, rendendo novos juros ("juros sobre juros"). | Fazem o dinheiro crescer exponencialmente ao longo do tempo, sendo o maior aliado do investidor no longo prazo. |
| **Custo Efetivo Total (CET)** | Percentual que mostra o custo real de um empréstimo ou financiamento, incluindo juros, tarifas, impostos e encargos. | Permite comparar propostas de diferentes bancos de forma justa, revelando taxas e custos ocultos. |
| **Agente de Custódia** | Instituição intermediária (corretora ou banco) responsável por administrar a conta do investidor e liquidar as operações. | É obrigatório cadastrar-se em um agente autorizado para conseguir operar no Tesouro Direto ou na Bolsa. |
| **Bolsa de Valores** | Ambiente regulado e eletrônico onde investidores compram e vendem valores mobiliários (ações, fundos, etc.). | Funciona como um mercado secundário seguro, garantindo transparência de preços em tempo real. |

---

### Questionário de Autoavaliação (Resultado do Prompt 3)

* **Pergunta 1:** Qual é a relação geral entre a rentabilidade prometida por um investimento e o risco de perda associado a ele?
  * A) Quanto maior a rentabilidade prometida, menor será o risco de perder a quantia aplicada.
  * B) O risco e a rentabilidade são fatores independentes, pois investimentos com total segurança podem oferecer a maior rentabilidade do mercado.
  * C) Quanto maior a rentabilidade prometida, maior o risco de perder a quantia aplicada, significando que o que se ganha em segurança perde-se em rentabilidade.
  * D) Investimentos de renda fixa, por garantirem uma taxa de juros predefinida, anulam totalmente qualquer risco de perda, independentemente da rentabilidade.
  * *Resposta Correta:* **C**
  * *Justificativa:* A relação é diretamente proporcional. As fontes explicam que: *"Em geral, quanto maior a rentabilidade prometida, maior o risco de perder a quantia aplicada. Em outras palavras, o que ganhamos em segurança perdemos em rentabilidade e vice-versa"*.

* **Pergunta 2:** Considerando a relação entre risco e retorno, como diferentes tipos de investimentos se comportam na prática?
  * A) A caderneta de poupança e o tesouro direto são classificados como investimentos de menor risco.
  * B) As ações são consideradas investimentos de menor risco por serem reguladas pela Bolsa de Valores.
  * C) A renda variável não oferece riscos, pois a remuneração já é dimensionada no momento em que a aplicação é feita.
  * D) Qualquer investimento, seja de renda fixa ou variável, oferece o mesmo nível de risco de perda financeira para o investidor.
  * *Resposta Correta:* **A**
  * *Justificativa:* O material cita diretamente: *"Exemplos de investimentos de menor risco são a caderneta de poupança e o tesouro direto, desde que você fique de posse do título e o desconte na data de seu vencimento, enquanto as ações são consideradas investimentos de maior risco"*.

* **Pergunta 3:** Como a relação entre risco e retorno influencia as escolhas dos diferentes perfis de investidores (conservador, moderado e arrojado)?
  * A) O investidor de perfil arrojado privilegia a segurança absoluta, evitando qualquer tipo de oscilação em seus investimentos.
  * B) O investidor de perfil conservador privilegia a segurança e tenta diminuir ao máximo o risco de perdas, o que significa que ele aceita ter uma rentabilidade menor.
  * C) O investidor de perfil moderado não se preocupa com o equilíbrio entre segurança e rentabilidade, assumindo os maiores riscos possíveis.
  * D) O perfil conservador é aquele que busca sempre o máximo de rentabilidade, independentemente de estar exposto a grandes riscos.
  * *Resposta Correta:* **B**
  * *Justificativa:* O texto define que o perfil Conservador: *"privilegia a segurança e faz todo o possível para diminuir o risco de perdas, aceitando, inclusive, uma rentabilidade menor"*.

---

## 5. Conclusão e Análise Crítica

A utilização do NotebookLM atuou como um excelente filtro contra alucinações, uma vez que a ancoragem do modelo restringiu as respostas aos dados emitidos pelo Banco Central e pela CVM. A experiência demonstrou que a IA acelera o mapeamento de conteúdos densos, mas exige que o estudante atue ativamente na curadoria e no refinamento das instruções para obter um material de revisão verdadeiramente produtivo.
