# Projeto 2: Aprendizagem supervisionada

## Criando um Sistema de Intervenção para Estudantes
### Instalação
Este projeto requer **Python 2.7** e as seguintes bibliotecas Python instaladas:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org/)
- [scikit-learn](http://scikit-learn.org/stable/)

Você também precisará ter software instalado para rodar e executar um [iPython Notebook](http://ipython.org/notebook.html)

A Udacity recomenda que os estudantes instalem [Anaconda](https://www.continuum.io/downloads), uma distribuição Python que contém todas as bibliotecas e software necessários para este projeto. 

### Código
Um modelo de código é fornecido no arquivo notebook `student_intervention_PT.ipynb`. Mesmo que parte do código já tenha sido fornecida para ajudá-lo a começar, você precisará implementar funcionalidades adicionais em alguns pontos para conseguir completar o projeto com sucesso.

### Execução
Em um terminal ou janela de comando, navegue até o diretório raiz de projeto `student_intervention/` (que contém este README) e execute os seguintes comandos:

```ipython notebook student_intervention_PT.ipynb```  
```jupyter notebook student_intervention_PT.ipynb```

Isso abrirá o o software e arquivo de projeto Jupyter Notebook em seu navegador.

## Dados
Os dados usados neste projeto estão incluídos em `student-data.csv`. O conjunto de dados possui os seguintes atributos:

- `school` : escola do estudante (binário: "GP" ou "MS")
- `sex` : sexo do estudante (binário: "F" - feminino ou "M" - masculino)
- `age` : idade do estudante (numérico: de 15 a 22)
- `address` : tipo de endereço do estudante (binário: "U" - urbano ou "R" - rural)
- `famsize` : tamanho da família (binário: "LE3" - até 3 pessoas ou "GT3" - mais de 3)
- `Pstatus` : situação de coabitação parental (binário: "T" - vivendo juntos ou "A" - separados)
- `Medu` : nível de escolaridade da mãe (numérico: 0 - nenhum,  1 - educação primária (até quarto ano), 2 - quinto a nono ano, 3 - ensino médio ou 4 - educação superior)
- `Fedu` : nível de escolaridade do pai (numérico: 0 - nenhum,  1 - educação primária (até quarto ano), 2 - quinto a nono ano, 3 - ensino médio ou 4 - educação superior)
- `Mjob` : profissão da mãe (nominal: "teacher" (professora), "health" (relacionado à saúde), "services" (ex. cargo administrativo ou policial), "at_home" (de casa) ou "other" (outros))
- `Fjob` : profissão do pai (nominal: "teacher" (professor), "health" (relacionado à saúde), "services" (ex. cargo administrativo ou policial), "at_home" (de casa) ou "other" (outros))
- `reason` : razão para escolher a escola (nominal: "home" (proximidade), "reputation" (reputação), "course" (preferência do curso) ou "other" (outro))
- `guardian` : responsável pelo estudante (nominal: "mother" (mãe), "father" (pai) ou "other" (outro))
- `traveltime` : tempo do trajeto casa-escola (numérico: 1 - <15 min., 2 - 15 a 30 min., 3 - 30 min. a 1 hora, ou 4 - >1 hora)
- `studytime` : tempo semanal de estudo (numérico: 1 - <2 horas, 2 - 2 a 5 horas, 3 - 5 a 10 horas, ou 4 - >10 horas)
- `failures` : número de reprovações passadas (numérico: n se 1<=n<3, senão 4)
- `schoolsup` : suporte educacional extra (binário: sim ou não)
- `famsup` : suporte educacional familiar (binário: sim ou não)
- `paid` : classes pagas extras dentre as matérias curriculares (Matemática ou Português) (binário: sim ou não)
- `activities` : atividades extra-curriculares (binário: sim ou não)
- `nursery` : frequentou educação infantil (binário: sim não)
- `higher` : pretende cursar educação superior (binário: sim ou não)
- `internet` : Acesso à internet em casa (binário: sim ou não)
- `romantic` : em um relacionamento afetivo (binário: sim ou não)
- `famrel` : qualidade das relações familiares (numérico: de 1 - muito ruim a 5 - excelente)
- `freetime` : tempo livre depois da escola (numérico: de 1 - muito baixo a 5 - muito alto)
- `goout` : frequência de saída com os amigos (numérico: de 1 - muito baixa a 5 - muito alta)
- `Dalc` : consumo de álcool durante dias úteis (numérico: de 1 - muito baixo a 5 - muito alto)
- `Walc` : consumo de álcool durante os fins de semana (numérico: de 1 - muito baixo a 5 - muito alto)
- `health` : estado atual de saúde (numérico: de 1 - muito ruim a 5 - muito bom)
- `absences` : número de faltas na escola (numérico: de 0 a 93)
- `passed` : se o estudante passou no exame final (binário: sim ou não)