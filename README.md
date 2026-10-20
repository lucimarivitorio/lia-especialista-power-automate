Projeto acadêmico de um segundo cérebro com a LIA, especialista em Microsoft Power Automate.

# LIA — Especialista em Microsoft Power Automate

## 1. Tema e objetivo

**Tema:** Microsoft Power Automate — automação de processos e diagnóstico de fluxos.

**Objetivo:** A LIA tem como objetivo apoiar a identificação e a automatização de processos manuais e repetitivos com o Microsoft Power Automate, ajudando a construir automações úteis, seguras e confiáveis. Para isso, consulta as fontes selecionadas, explica conceitos, auxilia no diagnóstico de problemas e orienta a construção, os testes e a validação dos fluxos com clareza e fundamentação documental.

## 2. Justificativa do projeto

Tarefas manuais e repetitivas podem consumir tempo e aumentar a possibilidade de erros. Ao mesmo tempo, compreender os recursos do Microsoft Power Automate, configurar fluxos e investigar falhas exige conhecimento técnico e consulta a materiais confiáveis.

Este projeto explora a criação de um segundo cérebro especializado, utilizando o NotebookLM para organizar fontes e configurar uma persona capaz de apoiar o estudo do Power Automate.

A LIA foi desenvolvida para explicar conceitos, orientar procedimentos e estruturar investigações de problemas com base nos materiais disponíveis. Seu desempenho é avaliado por meio de perguntas que exploram explicações conceituais, orientações de configuração e diagnóstico de falhas.

## 3. Fontes utilizadas e critérios de confiança

As fontes foram selecionadas para combinar uma diretriz de comportamento específica com documentação técnica sobre o Microsoft Power Automate.

- [Criar seu primeiro fluxo — Microsoft Learn](https://learn.microsoft.com/pt-br/training/)
- [Criar um fluxo de nuvem no Power Automate — Microsoft Learn](https://learn.microsoft.com/pt-br/power-automate/getting-started)
- [Introdução ao Power Automate — Microsoft Learn](https://learn.microsoft.com/pt-br/training/powerplatform/power-automate)
- [Solucionar problemas de erros em fluxos de nuvem — Microsoft Learn](https://learn.microsoft.com/pt-br/power-automate/troubleshoot-flow-errors)
- [Corrigir falhas de conexão em fluxos de nuvem — Microsoft Learn](https://learn.microsoft.com/pt-br/power-automate/fix-connection-failures)
- [Referência de códigos de erro — Microsoft Learn](https://learn.microsoft.com/pt-br/power-automate/error-reference)
- [Solucionar problemas de gatilhos — Microsoft Learn](https://learn.microsoft.com/pt-br/troubleshoot/power-platform/power-automate/flow-run-issues/triggers-troubleshoot)
- `LIA — Instruções Completas de Funcionamento.pdf`
- `power-automate.pdf`
- `power-automate-guidance.pdf`

**Critério de confiança:** priorizar a documentação oficial da Microsoft para afirmações técnicas sobre o Power Automate e utilizar o PDF de instruções para definir o comportamento esperado da persona.

A presença de uma fonte no notebook não garante que toda resposta esteja correta. É necessário avaliar a pertinência da fonte, a correspondência entre a afirmação e o trecho citado e a clareza com que a LIA reconhece eventuais limitações.

## 4. Diretriz de comportamento da LIA

A LIA recebeu uma diretriz de comportamento voltada à precisão técnica, à rastreabilidade das respostas e à segurança na orientação de automações. As principais regras estabelecidas foram:

- Consultar o documento de instruções antes de responder a questões técnicas.
- Priorizar as fontes disponíveis e a documentação oficial pertinente.
- Não inventar funcionalidades, propriedades, resultados de testes ou comportamentos da plataforma.
- Diferenciar fatos confirmados, hipóteses e informações ainda necessárias.
- Solicitar contexto adicional quando a pergunta não contiver dados suficientes para uma orientação segura.
- Apresentar procedimentos de forma organizada e verificável.
- Indicar fontes diretamente relacionadas às afirmações técnicas.
- Avaliar riscos de alterações, reprocessamento e possíveis efeitos colaterais antes de recomendar ações.
- Não afirmar que acessou o ambiente do usuário nem que executou testes sem evidências.
- Reconhecer limitações e revisar criticamente respostas quando houver sinais de inconsistência, falta de fundamentação ou excesso de certeza.

A diretriz busca fazer da LIA um apoio ao estudo e ao diagnóstico, e não apenas um gerador de respostas plausíveis.

## 5. Perguntas realizadas, respostas e avaliação dos testes

Foram realizados três testes para avaliar diferentes capacidades da LIA: explicação de conceitos, orientação para construção de uma automação e investigação de uma falha hipotética.

### Teste 1 — Diferença entre gatilhos e ações

**Pergunta realizada:** com base exclusivamente nas fontes disponíveis no notebook, explicar a diferença entre um gatilho e uma ação no Microsoft Power Automate, apresentar um exemplo simples de automação de uma tarefa manual e repetitiva e identificar as fontes que sustentam a explicação.

**Objetivo:** verificar se a LIA explica conceitos fundamentais, apresenta um exemplo prático e identifica as fontes utilizadas.

**Resumo da resposta:** a LIA explicou que o gatilho inicia um fluxo quando ocorre um evento, enquanto uma ação representa uma operação executada durante o fluxo. Como exemplo, apresentou um cenário em que o recebimento de um e-mail pode iniciar etapas posteriores, como salvar um arquivo e enviar uma notificação.

**Resultado:** aprovado com ressalvas.

**Análise:** a resposta diferenciou os conceitos, apresentou um exemplo prático e listou fontes documentais. Entretanto, a fundamentação depende da conferência das citações exibidas no NotebookLM.

**Limitação:** a identificação de fontes pelo nome não substitui a verificação de que os trechos citados sustentam efetivamente as afirmações.

**Fontes mencionadas na resposta:** *Criar seu primeiro fluxo — Training | Microsoft Learn*; *Criar um fluxo de nuvem no Power Automate — Power Automate | Microsoft Learn*; `power-automate.pdf`; `power-automate-guidance.pdf`; *Introdução ao Power Automate — Training | Microsoft Learn*; e *Exercício: criar fluxos recorrentes — Training | Microsoft Learn*.

**Evidências:** 
- `evidenciasteste_01_gatilhos_acoes.png`
- `evidenciasteste_01.1_gatilhos_acoes.png`

### Teste 2 — Orientação sobre a construção de uma automação

**Pergunta realizada:** orientar a construção de um fluxo que registre automaticamente respostas do Microsoft Forms em uma tabela existente do Excel, indicando o gatilho, as ações, os pré-requisitos e a sequência de configuração. A LIA também foi orientada a identificar configurações que precisariam ser confirmadas no ambiente e a não presumir que o fluxo já havia sido criado ou testado.

**Objetivo:** avaliar se a LIA consegue apresentar uma orientação técnica organizada para uma possibilidade de automação envolvendo Microsoft Forms, Power Automate e Excel.

**Resumo da resposta:** a LIA indicou o gatilho de recebimento de uma nova resposta no Microsoft Forms, a ação de obtenção dos detalhes da resposta e a ação de inserção de uma linha na tabela do Excel. Também apresentou pré-requisitos, etapas de configuração, mapeamento de campos e procedimentos sugeridos para testar o fluxo.

**Resultado:** aprovado com ressalvas.

**Análise:** a resposta apresentou uma sequência de configuração coerente com o objetivo proposto, destacou dependências importantes e indicou aspectos que precisariam ser confirmados no ambiente.

**Limitação:** a orientação foi avaliada com base na resposta textual. O fluxo não foi implementado nem executado. As fontes e citações específicas precisam ser conferidas na resposta original do NotebookLM antes de serem registradas como comprovadas.

**Fontes relacionadas:** registrar aqui os nomes das fontes efetivamente citadas na resposta do teste 2, após conferir a interface do NotebookLM.

**Evidências:**
- `evidenciasteste_02_orientacao_automacao.png`

### Teste 3 — Diagnóstico hipotético de falha em uma automação

**Pergunta realizada:** investigar um fluxo do Microsoft Power Automate que deveria registrar respostas do Microsoft Forms em uma tabela do Excel, mas não está realizando o registro, sem dispor inicialmente do código do erro ou dos detalhes da última execução. A LIA foi orientada a apresentar possíveis causas como hipóteses, indicar evidências a verificar e não presumir acesso ao ambiente.

**Objetivo:** verificar se a LIA consegue orientar uma investigação estruturada sem afirmar uma causa definitiva sem evidências.

**Resumo da resposta:** a LIA organizou possíveis causas relacionadas ao acionamento do gatilho, às conexões, à configuração da tabela do Excel e ao processamento dos dados. Também sugeriu verificar o histórico de execuções, os detalhes das ações e as mensagens de erro.

**Resultado:** aprovado com ressalvas.

**Análise:** a resposta separou fatos observados de hipóteses, propôs uma sequência de diagnóstico e solicitou informações adicionais sobre as execuções e as mensagens de erro.

Entretanto, algumas interpretações foram apresentadas de forma categórica. A ausência de execuções no histórico ou o status de sucesso de uma execução, isoladamente, não confirmam uma causa específica. É necessário examinar os detalhes da execução, as saídas das ações e o registro no arquivo de destino.

**Limitação:** o diagnóstico foi avaliado com base em uma situação hipotética. Nenhum fluxo real foi inspecionado ou corrigido. As fontes e citações específicas precisam ser conferidas na resposta original do NotebookLM.

**Fontes relacionadas:** registrar aqui os nomes das fontes efetivamente citadas na resposta do teste 3, após conferir a interface do NotebookLM.

**Evidências:**
- `evidenciasteste_03_diagnostico.png`
- `evidenciasteste_03.1_diagnostico.png`

## 6. Materiais complementares do projeto

Além das fontes utilizadas para orientar as respostas, o projeto pode incluir materiais produzidos ou exportados durante o uso do NotebookLM.

| Material | Formato | Finalidade |
|---|---|---|
| Mapa mental | PNG | Apresentar visualmente os conceitos organizados pelo notebook. |
| Infográfico | PNG | Resumir o conteúdo estudado. |
| Arquitetura de Automação com Power Automate: Do Fluxo à Governança | PDF | Material complementar de estudo sobre automação. |
| Dominando o Power Automate | MP4 | Material audiovisual complementar. |

Esses arquivos são materiais complementares do projeto. Não substituem a documentação técnica oficial utilizada para verificar as afirmações da LIA.

## 7. Link do notebook compartilhado

**NotebookLM — LIA, Especialista em Microsoft Power Automate:**

[ Abrir o notebook da LIA no NotebookLM ](https://notebook.google.com/notebook/814d25b7-804b-48e2-a4f8-e4aa58920dd1)

## 8. Organização dos arquivos do repositório

A estrutura proposta para os arquivos é:

```text
lia-especialista-power-automate/
├── README.md
├── documentacao/
│   └── objetivo_e_justificativa.docx
├── fontes/
│   ├── LIA_Instrucoes_Completas_de_Funcionamento.pdf
│   └── outros_materiais_de_referencia.pdf
├── materiais_gerados/
│   ├── mapa_mental.png
│   ├── slides.pdf
│   ├── Arquitetura_de_Automacao_Power_Automate.pdf
│   └── Dominando_o_Power_Automate.mp4
└── evidencias/
    ├── teste_01_gatilhos_acoes_1.png
    ├── teste_01_gatilhos_acoes_2.png
    ├── teste_02_orientacao_automacao.png
    ├── teste_03_diagnostico.png
    └── teste_03_diagnostico_2.png
```
