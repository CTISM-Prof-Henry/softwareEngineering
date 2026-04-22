# Extreme Programming

Extreme Programming (abreviado para XP em inglês, de eXtreme Programming), assim como o SCRUM, é um método ágil de
desenvolvimento de software. Proposto inicialmente por Kent Beck em 1999, o Extreme Programming é um método que enfatiza
a comunicação, simplicidade, feedback e coragem. A ideia é pegar as boas práticas de desenvolvimento de software e 
levá-las ao extremo.

<span>
<img alt="ciclos do extreme programming" src="../imagens/extreme_programming.png" width="500px">
<img alt="práticas do extreme programming" src="../imagens/extreme_programming_pr%C3%A1ticas.png" width="500px">
</span>

O XP pode ser dividido em dois principais eixos: seus **valores** e suas **atividades**.

## Valores

* Comunicação
* Simplicidade
* Coragem
* Feedback
* Respeito

## Atividades

### Codificação

Segundo o XP, a codificação é a atividade mais importante do desenvolvimento de software. O código é o artefato mais
importante do desenvolvimento de software, e a codificação pode ser usada para comunicação entre membros da equipe.

Se a revisão de código-fonte é uma boa prática de desenvolvimento, então a revisão _levada ao extremo_ leva a 
**programação em pares.**

### Testes

Se poucos testes de software têm o potencial de capturar poucos bugs, então muitos testes de software têm o potencial
de capturar muitos bugs. Portanto, no XP, a **cobertura de testes** deve ser extensa, e nenhuma nova funcionalidade é 
implementada antes de um teste unitário ser implementado antes. Bugs não são falhas no software, mas sim testes que não
foram implementados ainda.

No XP também estão presentes **testes de aceitação**, para verificar se o software atende aos requisitos do cliente, e *
*testes de integração**, para verificar se os diferentes componentes do software estão integrados corretamente.

### Escuta

A comunicação entre cliente e desenvolvedores é fundamental para o sucesso do desenvolvimento de software. O XP enfatiza
a importância de ouvir o cliente, para entender suas necessidades e expectativas, e também de ouvir os membros da
equipe, para entender suas dificuldades e sugestões.

Levado ao extremo, a escuta leva a **reuniões diárias** (as _dailies), onde os membros da equipe se reúnem para discutir
o progresso do desenvolvimento, os obstáculos encontrados e as próximas tarefas a serem realizadas.

### Design

O design do software deve ser simples, e deve ser feito de forma iterativa e incremental. O XP enfatiza a importância de
fazer o design do software de forma colaborativa, envolvendo todos os membros da equipe, e também de fazer o design do
software de forma evolutiva, ou seja, o design do software deve evoluir ao longo do desenvolvimento, e não deve ser
definido de forma rígida no início do desenvolvimento.

Levado ao extremo, isto significa não implementar recursos de software até que sejam necessários. Por exemplo, _add-ons_
devem ser postergados no desenvolvimento até que sejam realmente necessários.

## Regras

Adaptado da [Wikipedia](https://en.wikipedia.org/wiki/Extreme_programming):

* **Programação**
  * O cliente está sempre disponível
  * Codifique primeiro os testes unitários
  * Apenas uma dupla integra o código por vez
  * Deixe a otimização para o final
  * Sem horas extras

* **Testes**
  * Todo o código deve ter testes unitários
  * Todo o código deve passar em todos os testes unitários antes de ser liberado.
  * Quando um bug é encontrado, os testes são criados antes que o bug seja corrigido (um bug não é um erro de lógica;
    é um teste que não foi escrito)
  * Os testes de aceitação são executados frequentemente e os resultados são publicados