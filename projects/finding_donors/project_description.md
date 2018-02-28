# Conteúdo: Aprendizagem supervisionada
## Projeto: Encontrando doadores para a CharityML

## Visão geral do projeto
Neste projeto, você aplicará técnicas de aprendizagem supervisionada e seu raciocínio analítico sobre os dados coletados pelo censo dos Estados Unidos para ajudar a CharityML (uma instituição de caridade fictícia) a identificar as pessoas com maior probabilidade de doar à causa deles. Primeiro, você fará uma exploração para saber como os dados do censo são gravados. Em seguida, aplicará uma série de transformações e técnicas de pré-processamento para manipular os dados e organizá-los em um formato com o qual poderá trabalhar. Depois, avaliará vários modelos de aprendizagem supervisionada de sua escolha sobre os dados para definir qual é o mais adequado para a solução. Depois disso, otimizará o modelo que você selecionou e o apresentará como sua solução para a CharityML. Por fim, você explorará o modelo escolhido e suas predições por debaixo dos panos para avaliar seu desempenho considerando os dados disponibilizados.
preço de venda previsto para as suas estatísticas.

## Destaques do projeto
Este projeto foi desenvolvido de modo que você se familiarize com os muitos algoritmos de aprendizagem supervisionada disponíveis em sklearn e também para mostrar como cada modelo funciona e performa em um determinado tipo de dado. É importante em machine learning compreender exatamente quando e onde um determinado algoritmo deve ser usado e quando deve ser evitado.

O que você aprenderá ao concluir este projeto:
- Como identificar se o pré-processamento é necessário e como aplicá-lo.
- Como estabelecer uma referência para uma solução do problema.
- O que cada um dos vários algoritmos de aprendizagem supervisionada realiza, considerando um conjunto de dados específico.
- Como avaliar se um candidato a modelo de solução é adequado ao problema.

## Requisitos de software

Este projeto utiliza os seguintes software e bibliotecas Python:

- [Python 2.7](https://www.python.org/download/releases/2.7/)
- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [Matplotlib](http://matplotlib.org/)

Você também precisará ter um software instalado para rodar e executar um [notebook Jupyter](http://ipython.org/notebook.html)

Se você ainda não tem o Python instalado, é altamente recomendado que instale a distribuição [Anaconda](http://continuum.io/downloads), que já tem os pacotes acima incluídos. Certifique-se de selecionar o instalador Python 2.7, não o 3.x.

## Iniciando o projeto

Para esta tarefa, você pode achar a pasta `finding_donors`, contendo os arquivos de projeto necessários, no [GitHub de projetos de machine learning](https://github.com/udacity/br-machine-learning), dentro da pasta `projects`. Você pode baixar todos os arquivos de projetos que iremos usar neste programa Nanodegree diretamente desse repositório. Certifique-se de usar a versão mais recente dos arquivos ao concluir um projeto.

Este projeto contém três arquivos:

- `finding_donors_PT.ipynb`: Este é o arquivo principal com o qual você trabalhará em seu projeto.
- `census.csv`: O conjunto de dados do projeto. Você carregará esses dados no notebook.
- `visuals.py`: Um arquivo Python que contém o código de visualização que é executado nos bastidores. Não o modifique

No terminal ou janela de comando, navegue até a pasta contendo os arquivos do projeto; em seguida, use o comando `jupyter notebook finding_donors_PT.ipynb` para abrir uma janela ou aba do navegador e trabalhar com seu notebook. Alternativamente, você pode usar o comando `jupyter notebook` ou `ipython notebook` e navegar para o arquivo notebook na janela do navegador que abrir. Siga as instruções no notebook e responda a todas as perguntas apresentadas para concluir o projeto com sucesso. Um arquivo **README** também foi fornecido com os arquivos de projeto, contendo as instruções ou informações adicionais necessárias. 

## Enviando o projeto

### Avaliação
Seu projeto será avaliado por um revisor da Udacity, de acordo com a **<a href="https://review.udacity.com/#!/rubrics/1499/view" target="_blank">rubrica do projeto Encontrando doadores para a CharityML</a>**. Lembre-se de revisar esta rubrica cuidadosamente e autoavaliar seu projeto antes de enviá-lo. Todos os critérios encontrados nesta rubrica devem *atender às especificações* para que você seja aprovado.

### Arquivos para envio
Quando estiver pronto para enviar o projeto, reúna os arquivos a seguir e os comprima em um único arquivo para upload. Alternativamente, você pode fornecer os seguintes arquivos no seu repositório GitHub em uma pasta chamada `finding_donors` para facilitar o acesso:
 - O arquivo notebook `finding_donors_PT.ipynb`, com todas as perguntas respondidas e todas as células de código executadas e mostrando a saída.
 - Uma exportação **HTML** do notebook do projeto, com o nome **report.html**. Este arquivo *deve* estar presente para o seu projeto ser avaliado.

Assim que você tiver reunido todos esses arquivos e revisado sua rubrica, prossiga para a página de envio do projeto.

### Estou pronto!
Quando estiver pronto para enviar seu projeto, clique no botão ***Enviar projeto***, no final da página.

Caso tenha problemas de envio ou queira conferir o status de sua entrega, mande um e-mail para **suporte@udacity.com** ou acesse os <a href="http://discussions.udacity.com" target="_blank">fóruns de discussão</a>.

### E agora?
Você receberá um e-mail assim que seu projeto tiver um feedback do revisor. Enquanto isso, revise seu próximo projeto e fique à vontade para começá-lo ou começar os cursos que o apoiam!
