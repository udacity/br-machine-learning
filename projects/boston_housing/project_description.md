# Conteúdo: Modelo de avaliação e validação
## Projeto: Prevendo o preço de imóveis de Boston

## Visão geral do projeto
Neste projeto, você aplicará conceitos básicos de Machine Learning em dados coletados de preços de casas em Boston, em Massachusetts, para prever o preço de venda de uma casa nova. Primeiro, você irá explorar os dados para obter atributos importantes  e estatísticas descritivas sobre o conjunto de dados. Depois, dividirá adequadamente os dados entre dois subconjuntos, o de testes e o de treinamento, e determinará uma métrica adequada para esse problema. Você, então, analisará o desempenho de um algoritmo de aprendizagem com parâmetros variados e tamanho do conjunto de treinamento. Isso permitirá que você escolha o modelo ótimo que melhor generaliza os dados desconhecidos. Por último, você testará o modelo ótimo em uma nova amostra e comparará os preços de venda previstos com as suas estatísticas.

## Destaques do projeto
Este projeto foi projetado para que você se familiarize em trabalhar com conjuntos de dados em Python e aplicar técnicas básicas de Machine Learning utilizando NumPy e Scikit-Learn. Antes de saber usar muitos dos algoritmos disponíveis na biblioteca sklearn, será de grande ajuda, primeiro, praticar análise e interpretação do desempenho de seu modelo.

O que você aprenderá ao concluir este projeto:

- Como utilizar o NumPy para investigar os features latentes de um conjunto de dados.
- Como analisar vários gráficos de desempenho de aprendizagem para variância e viés.
- Como determinar o modelo que faz as melhores estimativas para dados desconhecidos.
- Como avaliar o desempenho do modelo em dados desconhecidos utilizando dados anteriores.

## Descrição
O mercado imobiliário de Boston é altamente competitivo e você quer ser o melhor corretor de imóveis da região. Para competir com seus colegas, você decidiu elencar alguns conceitos básicos de Machine Learning para ajudar você e seu cliente a acharem o melhor preço de venda para a casa dele. Com sorte, você se deparou com o conjunto de dados de habitação de Boston, que contém dados agregados de várias características para casas das comunidades da Grande Boston, incluindo o valor médio das casas para cada uma das regiões. Sua tarefa é construir um modelo ótimo baseado na análise das estatísticas com as ferramentas disponíveis. Esse modelo será, então, usado para estimar o melhor preço de venda para a casa de seus clientes.

## Software e bibliotecas
Este projeto usará o seguinte software e bibliotecas de Python:

- [Python 2.7](https://www.python.org/download/releases/2.7/)
- [NumPy](http://www.numpy.org/)
- [pandas](http://pandas.pydata.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [matplotlib](http://matplotlib.org/)
- [Jupyter Notebook](http://ipython.org/notebook.html)

Caso você não tenha o Python instalado ainda, é altamente recomendado que instale a distribuição [Anaconda](http://continuum.io/downloads) de Python, que já tem os pacotes acima inclusos, além de outros. Certifique-se de que você selecionou o instalador do Python 2.7, e não o instalador do Python 3.x.

## Começando o projeto
Para essa tarefa, você encontrará o arquivo `boston_housing.zip`, que contém os arquivos necessários do projeto para download na seção Recursos. *Você também pode visitar nosso [GitHub de projetos de Machine Learning](https://github.com/udacity/br-machine-learning) para ter acesso a todos os projetos disponíveis para este Nanodegree.*

Este projeto contém três arquivos:

- `boston_housing_PT.ipynb`: esse é o arquivo principal, em que você irá executar seu projeto.
- `housing.csv`: o conjunto de dados do projeto. Você vai carregar esses dados no Notebook.
- `visuals.py`: esse script de Python contém funções auxiliares que criarão as visualizações necessárias.

No Terminal ou no prompt de comando, navegue até a pasta que contém os arquivos do projeto e, então, utilize o comando `jupyter notebook boston_housing_PT.ipynb` para abrir uma nova janela ou aba do navegador para trabalhar com seu Notebook. Outra alternativa é utilizar o comando `jupyter notebook` ou `ipython notebook` e navegar até o arquivo do Notebook na janela do navegador que se abrir. Siga as instruções no Notebook e responda a cada uma das perguntas apresentadas para concluir o projeto com sucesso. O arquivo **README** também foi incluído e contém informações necessárias adicionais ou instruções para o projeto.

## Enviando o projeto
### Avaliação
Seu projeto será avaliado por um revisor da Udacity, de acordo com a [rubrica do projeto "Prevendo o preços de imóveis residenciais em Boston"](https://review.udacity.com/#!/rubrics/389/view). Certifique-se de ler a rubrica cuidadosamente e se autoavaliar antes de enviar o projeto. Seu projeto deve atender às especificações da rubrica para que seja aprovado.

### Arquivos para envio
Quando você estiver pronto para enviar o projeto, reúna os seguintes arquivos e os comprima em um único arquivo para upload. Outra maneira seria fornecer os seguintes arquivos no seu repositório do GitHub, em uma pasta nomeada `boston_housing`, para facilitar o acesso:

- O arquivo do Notebook `boston_housing.ipynb` com todas as perguntas respondidas e todos os blocos de código executados e exibindo a saída.
- Um arquivo **em HTML** com o nome `report.html` exportado do Notebook do projeto. Esse arquivo deve estar presente para que seu projeto seja avaliado.

Após reunir esses arquivos e ler a rubrica do projeto, vá até a página de envio. 

### Estou pronto!
Quando estiver pronto para enviar seu projeto, clique no botão **enviar projeto**, no fim desta página.

Caso você tenha qualquer problema ao enviar seu projeto ou deseje checar o status, envie um e-mail para **ml-suporte@udacity.com** ou visite nosso [fórum de discussão](https://discussions.udacity.com/c/nd009-model-evaluation-and-validation/nd009-br-predicting-boston-housing-prices).

### E agora?
Você receberá um e-mail assim que seu revisor tiver seu feedback pronto. Enquanto isso, leia seu próximo projeto e sinta-se à vontade para começá-lo - ou outros cursos que possam ajudar!