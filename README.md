# Azure Machine Learning - Automatizado
Vou guiá-lo através dos passos para criar um modelo de previsão com os pontos de extremidade configurados na plataforma Azure Machine Learning.

 <p align="center">
  <a href="#Tecnologias">Tecnologias</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#Documentação">Documentação</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
  <a href="#License">License</a>
</p>

![_1b5951ac-30f4-4064-8710-821e3d6a4382](https://github.com/augustomiller/ML_Azure_automated/assets/990877/7d2b8976-e462-4311-9af1-2240998715c1)

## Tecnologias

- [Azure Machine Learning](https://azure.microsoft.com/pt-br/free/machine-learning/search/?ef_id=_k_6cd5b45a590d1bb5cc07d1835eb85881_k_&OCID=AIDcmmzmnb0182_SEM__k_6cd5b45a590d1bb5cc07d1835eb85881_k_&msclkid=6cd5b45a590d1bb5cc07d1835eb85881)
- [Microsoft Copilot](https://copilot.microsoft.com/)
- [VS Code](https://code.visualstudio.com/)
- [Bash](https://www.gnu.org/software/bash/)
- [Git](https://git-scm.com/)

  ## Documentação

- [Azure ML Doc](https://learn.microsoft.com/en-us/azure/machine-learning/?view=azureml-api-2)
- [Microsoft Copilot Doc](https://learn.microsoft.com/en-us/microsoft-copilot-studio/)
- [VS Code Doc](https://code.visualstudio.com/Docs)
- [Bash Doc](https://www.gnu.org/software/bash/manual/bash.html)
- [Git](https://git-scm.com/doc)
- [Markdown Doc](https://google.github.io/styleguide/docguide/style.html)

## Vamos lá 🚀

1. Faça login em sua conta da Microsoft e crie um espaço de trabalho (workspace) no Azure Machine Learning Studio.
2. No ambiente do workspace, clique em “ML automatizado” no menu à esquerda.
3. Na próxima janela, clique em “+ Novo trabalho de ML automatizado”.
4. Preencha o formulário com os seguintes dados de configuração:
    - [x] Nome do trabalho: mslearn-bike-automl
    - [x] Nome do experimento: (Deixe em branco)
    - [x] Descrição: (Deixe em branco)
    - [x] Tags: (Deixe em branco)
5. Na próxima etapa, preencha os campos com os seguintes dados:
    - Tipo de tarefa e dados: Regressão
    - Conjunto de dados:
  - Crie um novo conjunto de dados com as seguintes configurações:
    - [x] Nome: bike-rentals
    - [x] Descrição: Dados históricos de aluguel de bicicletas
    - [x] Tipo: Tabular
    - [x] Fonte de dados: Selecione “De arquivos da Web”
    - [x] URL da Web: Dados de aluguel de bicicletas
  - Configurações:
    - [x] Formato de arquivo: Delimitado
    - [x] Delimitador: Vírgula
    - [x] Codificação: UTF-8
    - [x] Cabeçalhos de coluna: Somente o primeiro arquivo tem cabeçalhos
    - [x] Pular linhas: Nenhum
    - [x] Esquema: Incluir todas as colunas diferentes de Caminho
  - Configurações da tarefa:
    - [x] Tipo de tarefa: Regressão
    - [x] Coluna de destino: Aluguéis (inteiro)
    - [x] Métrica primária: Erro quadrático médio da raiz normalizada
    - [x] Explicar melhor modelo: Não selecionado
    - [x] Use todos os modelos suportados: Não selecionado (restrinja o trabalho para tentar apenas alguns algoritmos específicos)
    - [x] Modelos permitidos: Selecione apenas RandomForest e LightGBM
  - Limites:
      - [x] Máximo de tentativas: 3
      - [x] Máximo de tentativas simultâneas: 3
      - [x] Nós máximos: 3
      - [x] Limiar de pontuação métrica: 0,085 (se um modelo atingir uma pontuação métrica abaixo desse valor, o trabalho termina)
6. Clique em Criar para iniciar o trabalho de ML automatizado. O Azure Machine Learning irá treinar e avaliar modelos automaticamente com base nos parâmetros especificados.
Lembre-se de adaptar essas configurações conforme suas necessidades específicas. Boa sorte com seu projeto de previsão! 🚴‍♂️🔮

## License

<div align="center">
  
<p>This project is licensed under the MIT License. See the
  <a href="https://mit-license.org/">
    <img src="https://img.shields.io/static/v1?label=license&message=MIT&color=5965E0&labelColor=121214" alt="License"></a> file for details.</p>
<p>Made with&nbsp;💙 &nbsp;by Augusto Miller</p>
  
<div>
