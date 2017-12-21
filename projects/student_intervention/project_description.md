# Conteúdo: Aprendizagem supervisionada
## Projeto: Criando um Sistema de Intervenção para Estudantes

## Visão geral do projeto

Com o aumento do uso da tecnologia na educação, uma vasta quantidade de dados foi disponibilizada para avaliação e predição. Registros das atividades dos alunos, notas, interações com os professores e colegas, entre outros, agora são captados em tempo real por sistemas de gerenciamento de aprendizagem como o **Canvas** e o **Edmodo**. Esse fenômeno é particularmente forte em aulas à distância, que estão tornando-se populares até mesmo no Ensino Fundamental e Médio. Dentro de todos os níveis da educação, existe um impulso para aumentar a probabilidade de sucesso do aluno sem diluir a educação nem encorajar comportamentos que não vão melhorar os problemas na raiz. A taxa de graduação frequentemente é o critério preferencial, e os educadores procuram novas maneiras de predizer o sucesso ou o fracasso dos estudantes cedo o bastante para organizar intervenções eficazes.

## Descrição
Um distrito escolar da região tem como objetivo alcançar 95% de taxa de graduação até o fim da década, identificando alunos que precisam de intervenção antes que eles abandonem a escola. Como um engenheiro de software contratado pelo distrito escolar, sua tarefa é modelar os fatores que predizem a probabilidade de os alunos passarem na avaliação final do Ensino Médio, por meio de um sistema de intervenção baseado em técnicas de aprendizagem supervisionada. O conselho escolar pede que você encontre o modelo mais eficiente que tenha o menor custo computacional para poupar no orçamento. Você precisará analisar o conjunto de dados do desempenho escolar dos estudantes e desenvolver um modelo que preverá a probabilidade de um dado estudante passar, quantificando se uma intervenção é necessária.


## Software e bibliotecas
Este projeto usará o seguinte software e bibliotecas de Python:

- [Python 2.7](https://www.python.org/download/releases/2.7/)
- [NumPy](http://www.numpy.org/)
- [pandas](http://pandas.pydata.org/)
- [scikit-learn](http://scikit-learn.org/stable/)
- [matplotlib](http://matplotlib.org/)
- [Jupyter Notebook](http://ipython.org/notebook.html)

Caso você não tenha o Python instalado ainda, é altamente recomendado que instale a distribuição [Anaconda](http://continuum.io/downloads) de Python, que já tem os pacotes acima e mais alguns inclusos. Certifique-se de que você selecionou o instalador do Python 2.7 e não o instalador do Python 3.x.


## Começando o projeto
Para esta tarefa, você encontrará o arquivo `student_intervention.zip`, que contém os arquivos necessários do projeto para download na seção **Recursos**. *Você também pode visitar nosso [GitHub de projetos de machine learning](https://github.com/udacity/br-machine-learning) para ter acesso a todos os projetos disponíveis para este Nanodegree.*

Este projeto contém dois arquivos:

* `student_intervention_PT.ipynb`: este é o arquivo principal em que você executará sua tarefa do projeto.

* `student-data.csv`: o conjunto de dados do projeto. Você vai carregar esses dados no notebook.

No Terminal ou no Command Prompt, navegue até a pasta que contém os arquivos do projeto e, então, utilize o comando `jupyter notebook student_intervention_PT.ipynb` para abrir uma janela ou aba do navegador para trabalhar com seu notebook. Outra alternativa é utilizar o comando `jupyter notebook` ou `ipython notebook` e navegar até o arquivo do notebook na janela do navegador que abriu. Siga as instruções no notebook e responda a cada uma das perguntas apresentadas para concluir o projeto com sucesso. Um arquivo **README** também está incluído nos arquivos do projeto. Ele pode conter informações adicionais ou instruções para sua realização.

## Enviando o projeto
### Avaliação
Seu projeto será avaliado por um revisor da Udacity, de acordo com a [rubrica do projeto](https://review.udacity.com/#!/rubrics/388/view). Certifique-se de ler a rubrica cuidadosamente e autoavaliar-se antes de enviar o projeto: ele deve atender a **todas as especificações** listadas nela para ser aprovado.

### Arquivos para envio
Quando estiver pronto para enviar seu projeto, reúna os arquivos abaixo e os comprima em um único arquivo para upload. Outra maneira seria fornecê-los em seu repositório do GitHub, em uma pasta nomeada `student_intervention`, para facilitar o acesso.

- O arquivo do notebook `student_intervention_PT.ipynb `, com todas as perguntas respondidas e todos os blocos de código executados e exibindo a saída.
- Um arquivo **em HTML**, com o nome `report.html`, exportado do notebook do projeto. Esse arquivo deve estar presente para que seu projeto seja avaliado.

Após reunir esses arquivos e ler a rubrica do projeto, vá até a página de envio de projeto.

### Estou pronto!
Quando você estiver pronto para enviar seu projeto, clique no botão "Enviar Projeto", no fim desta página.

Caso você tenha qualquer problema ao enviar seu projeto ou queira checar o status de seu envio, envie um e-mail para ml-suporte@udacity.com ou visite nosso [fórum de discussão](https://discussions.udacity.com/c/nd009-supervised-learning/nd009-br-building-a-student-intervention-system).

### E agora?
Você receberá um e-mail assim que seu revisor tiver seu feedback pronto. Enquanto isso, leia seu próximo projeto e sinta-se à vontade para começá-lo ou assistir às próximas aulas!