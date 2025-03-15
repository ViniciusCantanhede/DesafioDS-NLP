# Desafio NLP para Extração de Informações Médicas - NeuralMed

## Sobre o Projeto

Este repositório contém minha solução para o desafio de Processamento de Linguagem Natural (NLP) proposto pela NeuralMed. O projeto implementa um sistema de extração de informações estruturadas a partir de documentos médicos não estruturados, utilizando técnicas de NER (Named Entity Recognition) e processamento baseado em prompts.

## Estrutura do Repositório

- **`/codigo`**: Contém o requirements.txt e o notebook Jupyter com a implementação completa do pipeline de NLP.
- **`/respostas`**: Documento com as respostas do Docs enviado para o desafio desafio.
- **`/documentacao`**: PDF produzido em LateX explicativo com a descrição completa do projeto, metodologia e resultados.

## Funcionalidades Implementadas

- Pré-processamento especializado para documentos médicos em diferentes formatos (HTML, RTF, texto plano)
- Sistema de reconhecimento de entidades nomeadas (NER) para identificação de:
  - Medicamentos
  - Procedimentos médicos
  - Dispositivos
  - Condições do paciente
  - Resultados de exames
- Extração via prompts estruturados para modelos de linguagem
- Comparação entre abordagens de NER e baseadas em prompts

## Pipeline de Desenvolvimento

O projeto segue um pipeline completo de desenvolvimento que inclui:

1. **Análise de dados**: Exploração dos documentos médicos e suas características
2. **Pré-processamento**: Limpeza e normalização dos textos
3. **Anotação**: Criação de um conjunto de dados anotado com entidades médicas
4. **Treinamento**: Desenvolvimento de um modelo NER especializado
5. **Avaliação**: Validação em exemplos representativos
6. **Aplicação**: Demonstração prática da extração de informações em novos documentos

## Tecnologias Utilizadas (Arquivo requirements.txt na pasta Codigo contém as versões)

- Python 3.11.11
- PyTorch
- Hugging Face Transformers
- NLTK
- Pandas
- RegEx
- Numpy

## Resultados

O modelo alcançou excelentes resultados na identificação de entidades médicas, com uma perda de validação final de 0.018560 após 3 épocas de treinamento. A abordagem combinada de NER e prompts demonstrou ser particularmente eficaz para extrair informações completas e estruturadas de textos médicos complexos.
