# Nanodegree Engenheiro de Machine Learning
# Aprendizagem por reforço
## Projeto: Ensinando um SmartCab a Dirigir

## Visão geral do projeto
Neste projeto, você aplicará técnicas de aprendizagem por reforço para um agente autocondutor em um mundo simplificado, auxiliando-o a chegar de maneira efetiva até seus destinos em um tempo específico. Primeiro, você investigará o ambiente em que o agente opera, implementando um algoritmo de direção bastante básico. Uma vez que o agente foi bem-sucedido ao operar dentro do ambiente, você então identificará cada possível estado em que o agente pode estar, considerando situações como semáforo e tráfego de sentido contrário em cada intersecção. Com os estados identificados, você implementará um algoritmo Q-Learning para o agente autocondutor ser guiado até seu destino dentro do tempo estimado. Por fim, você melhorará o algoritmo Q-Learning em que já trabalhou para encontrar a melhor configuração de aprendizagem e fatores de exploração que asseguram que o agente autocondutor chegue a seu destino com resultados positivos de forma consistente.

## Descrição
Em um futuro não tão distante, empresas de táxi dos Estados Unidos não mais contratarão condutores humanos para operar sua frota de veículos. Em vez disso, os táxis serão operados por agentes autocondutores — conhecido como _smartcabs_ ou táxis inteligentes —, transportando pessoas de um local para outro dentro das cidades onde essas empresas operam. Na maiorias das áreas metropolitanas, como Chicago, Nova Iorque e São Francisco, um crescente número de pessoas começou a confiar nos táxis inteligentes para chegar aonde precisam ir da maneira mais segura e eficiente possível. Embora táxis inteligentes tenham se tornado o transporte mais utilizado, surgem preocupações de que um agente autocondutor talvez não seja seguro ou eficiente como os condutores humanos, especialmente quando considerados os semáforos da cidade ou outros veículos. Para aliviar essa situação, sua tarefa como funcionário de uma empresa nacional de táxis é usar técnicas de aprendizagem por reforço para desenvolver uma demonstração de operação dos táxis inteligentes em tempo real e provar que ambas a segurança e a eficiência podem ser alcançadas.

## Requisitos de software
Este projeto usará os seguintes software e bibliotecas de Python:

- [Python 2.7](https://www.python.org/download/releases/2.7/)
- [NumPy](http://www.numpy.org/)
- [pandas](http://pandas.pydata.org/)
- [matplotlib](http://matplotlib.org/)
- [PyGame](http://pygame.org/)

Caso você não tenha o Python instalado ainda, é altamente recomendado que instale a distribuição [Anaconda](http://continuum.io/downloads), que já contém os pacotes acima inclusos, entre outros. Certifique-se de selecionar o instalador do Python 2.7, e não o instalador do Python 3.x. O pygame pode, então, ser instalando usando um dos seguintes comandos:

Mac:  `conda install -c https://conda.anaconda.org/quasiben pygame`  
Linux: `conda install -c https://conda.anaconda.org/tlatorre pygame`  
Windows:  `conda install -c https://conda.anaconda.org/prkrekel pygame`    

## Corrigindo problemas do PyGame
A biblioteca PyGame pode, em alguns casos, demandar alguns ajustes para funcionar corretamente para esse projeto. As funções do PyGame são necessárias para interface gráfica, mas não é obrigatória sua execução. No entanto, é muito mais fácil e divertido interagir com uma interface. Caso você tenha tido algum problema, veja alguns links úteis para te ajudar a resolver:
- [Getting Started](https://www.pygame.org/wiki/GettingStarted)
- [PyGame Information](http://www.pygame.org/wiki/info)
- [Google Group](https://groups.google.com/forum/#!forum/pygame-mirror-on-google-groups)
- [PyGame subreddit](https://www.reddit.com/r/pygame/)

### Problemas mais reportados por alunos
_"PyGame não instala na minha máquina; teve um problema na instalação."_
  
**Solução:** Como recomendado em outros projetos, a Udacity recomenda que você utilize a distribuição Python do Anaconda, o qual permite instalar o Pygame pelo comando `conda` específico.

_"Eu estou vendo uma tela preta enquanto o código executa; o *output* diz que que não pode carregar imagens de carros."_  
**Solução:** O código não executará corretamente se não for executado do diretório acima do `smartcab`. O diretório acima é aquele que contém o arquivo **README** e o notebook do projeto.

Se você ainda tiver problemas para executar o projeto com o PyGame, você pode utilizar o [fórum de discussão](https://discussions.udacity.com/c/nd009-reinforcement-learning) para ver postagens relacionadas com o seu problema. Você também pode procurar ajuda com os alunos no Slack.

## Começando o projeto
Para essa tarefa, você encontrará o arquivo smartcab.zip, que contém os arquivos necessários do projeto para download na seção "Recursos". *Você também pode visitar nosso**[GitHub de projetos de machine ,earning](https://github.com/udacity/br-machine-learning) para ter acesso a todos os projetos disponíveis para este Nanodegree.*
Este projeto contém três diretórios:
- `/logs/`: essa pasta contém todos os registros fornecidos pelo simulador quando pré-requisitos específicos são satisfeitos.
- `/images/`: essa pasta contém várias imagens de carros que podem ser utilizadas na interface gráfica do usuário. Você não precisará modificar nem criar nenhum arquivo nesse diretório.
- `/smartcab/`: essa pasta contém os scripts de Python que criarão o ambiente, a interface gráfica do usuário, a simulação e os agentes. Você não precisará modificar nem criar nenhum arquivo nesse diretório, exceto pelo agent.py.

Também há dois arquivos:
- `smartcab.ipynb`: este é o arquivo em que você vai responder às questões e fazer uma análise de seu trabalho.
- `visuals.py`: este script traz funções de visualização para complementar a análise. **Não o modifique**.

No `/smartcab/` há os seguintes arquivos:

- Modifique:
  - `agent.py` esse é o arquivo principal de Python em que você irá executar seu trabalho deste projeto.
- **Não o modifique**:
  - `environment.py`: esse arquivo de Python criará o ambiente do táxi inteligente.
  - `planner.py`: esse arquivo de Python criará um planejador de alto nível para que o agente siga em direção a um objetivo definido.
  - `simulation.py`: esse arquivo de Python criará a simulação e a interface gráfica do usuário.

### Compilando o código
No terminal ou na janela de comando, navegue até o nível superior do diretório (que contém os dois diretórios do projeto) e execute os seguintes comandos:

`python smartcab/agent.py` ou

`python -m smartcab.agent`

Isso executará o arquivo `agent.py` e o código do agente implementado dentro do ambiente.

O comando `jupyter notebook smartcab.ipynb` pode ser executado no mesmo diretório para abrir o notebook no navegador, para que você possa fazer a análise. Alternativamente, você pode usar o comando `jupyter notebook` dentro da pasta do projeto e usar a interface aberta no navegador para abrir o notebook. Siga as instruções nele contidas e responda a cada questão cuidadosamente para completar a implementação necessária de seu agente.

O arquivo **README** também foi incluído, contendo informações necessárias adicionais ou instruções para o projeto.

## Definições
### Ambiente
O táxi inteligente opera em uma cidade ideal, em forma de malha (similar à cidade de Nova Iorque), com ruas indo nas direções Norte-Sul e Leste-Oeste. Outros veículos certamente estarão presentes na cidade, mas não haverá pedestres para se preocupar. A cada intersecção há um semáforo que permite tráfego tanto na direção Norte-Sul como na Leste-Oeste. A cidade segue as regras norte-americanas de trânsito:
- No sinal verde, é permitido virar à esquerda se não houver nenhum tráfego no sentido contrário fazendo curva à direita ou indo reto pela intersecção.
- No sinal vermelho, curva à direita é permitido se não houver nenhum tráfego no sentido contrário se aproximando à sua esquerda, pela intersecção. Para entender como conduzir corretamente o tráfego de sentido contrário ao virar à esquerda, você pode assistir a [este vídeo oficial sobre educação de condutores](https://www.youtube.com/watch?v=TW0Eq2Q-9Ac) ou [esta palestra animada](https://www.youtube.com/watch?v=0EdkxI6NeuA).

### Entradas e saídas
Suponha que é atribuído ao táxi inteligente um plano de rota baseado na localização inicial e no destino do passageiro. A rota é dividida a cada intersecção em um ponto de navegação, e você pode assumir que o táxi inteligente, a qualquer instante, está em alguma interseção no mundo. Portanto, o próximo ponto de navegação para o destino, assumindo que o destino ainda não foi alcançado, é uma interseção distante em uma direção (Norte, Sul, Leste ou Oeste). O táxi inteligente tem apenas uma visão egocêntrica da interseção, que é: ele pode determinar o estado do semáforo adequado à sua direção, e se há um veículo na interseção para cada uma das direções contrárias. Para cada ação, o táxi inteligente pode ficar ocioso na interseção ou dirigir para a próxima interseção à esquerda, à direita ou em frente. Por último, cada viagem tem um tempo para alcançar o destino que diminui a cada ação tomada (os passageiros querem chegar a seu destino rapidamente). Se o tempo atribuído torna-se zero antes de alcançar o destino, a viagem falhou.

### Recompensas e objetivos
O táxi inteligente recebe uma recompensa a cada viagem bem-sucedida e também recebe recompensas menores por cada ação que ele executa com sucesso e obedecendo às leis de trânsito. O táxi inteligente recebe pequenas penalidade para cada ação incorreta, e grandes penalidades para cada ação que viole as leis de trânsito ou que cause um acidente com outro veículo. Baseado nas recompensas e penalidade que o táxi inteligente recebe, a implementação do agente autocondutor deverá aprender um política ótima para dirigir nas estradas da cidade enquanto obedece às leis de trânsito, evitando acidentes e alcançando o destino dos passageiros no tempo determinado.

### Avaliação
Esse projeto não é avaliado ou obrigatório. No entanto, você pode verificar os items da [rubrica do projeto](https://review.udacity.com/#!/rubrics/106/view) para ter certeza que você fez tudo corretamente.

### Estou pronto!
Caso tenha qualquer problema para desenvolver seu projeto envie um e-mail para **ml-suporte@udacity.com**, visite nosso [fórum de discussão](http://discussions.udacity.com/) ou compartilhe no Slack.