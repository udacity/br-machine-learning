# Nanodegree Engenheiro de Machine Learning
# Modelo de avaliação e validação
## Projeto: Prevendo o preço de imóveis de Boston

### Instalação

Este projeto requer **Python 2.7** (se você completar o projeto em Python 3.x, você precisará fazer o update do código em vários pontos, incluindo todos os prints relevantes) e as seguintes bibliotecas Python:

- [Python 2.7](https://www.python.org/download/releases/2.7/)
- [NumPy](http://www.numpy.org/)
- [pandas](http://pandas.pydata.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [matplotlib](http://matplotlib.org/)

Você também precisará ter software instalado para rodar e executar um [Jupyter Notebook](http://ipython.org/notebook.html)

Se você ainda não tem o Python instalado, é altamente recomendado que instale a distribuição [Anaconda](http://continuum.io/downloads), que já tem os pacotes acima incluídos. Certifique-se de selecionar o instalador Python 2.7, não o 3.x.

### Código

Um modelo do código é fornecido no arquivo notebook `boston_housing_PT.ipynb`. Você também precisará usar o arquivo Python `visuals.py` e o arquivo de dados `housing.csv` para completar seu trabalho. Mesmo que parte do código já tenha sido fornecida para ajudá-lo a começar, você precisará implementar funcionalidades adicionais em alguns pontos para conseguir completar o projeto com sucesso. Note que o código incluído em `visuals.py` foi feito para ser utilizado do jeito que está, sem manipulação por parte dos estudantes. Mas, se você estiver interessado em saber como as visualizações são criadas no notebook, fique à vontade para explorar esse arquivo Python.

### Execução
Em um terminal ou janela de comando, navegue até o diretório raiz de projeto `boston_housing/` (que contém este README) e execute os seguintes comandos:

```bash
ipython notebook boston_housing_PT.ipynb
```  
ou
```bash
jupyter notebook boston_housing_PT.ipynb
```

Isso abrirá o o software e arquivo de projeto Jupyter Notebook em seu navegador.

### Dados
O conjunto de dados do mercado imobiliário de Boston consiste em 489 pontos de dados, sendo que cada ponto possui 3 atributos. Este conjunto de dados é uma versão modificada do conjunto de dados do mercado imobiliário de Boston encontrado no [Repositório de machine learning da UCI](https://archive.ics.uci.edu/ml/datasets/Housing).

#### Atributos
1. `RM`: número médio de cômodos por casa
2. `LSTAT`: porcentagem da população considerada de baixa renda
3. `PTRATIO`: razão estudante/professor da cidade

#### Variável alvo
4. `MEDV`: valor mediano das casas