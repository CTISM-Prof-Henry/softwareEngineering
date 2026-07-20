# Engenharia de Requisitos

## O que é?

A Engenharia de Requisitos é a etapa do desenvolvimento na qual as funcionalidades do software são elencadas e 
priorizadas. 

Os requisitos de um software podem ser divididos em duas categorias: **requisitos de usuário** e **requisitos de 
sistema**. Os requisitos de usuário descrevem, em linguagem natural, as funcionalidades que o sistema deve apresentar,
sem se preocupar com detalhes de implementação (por exemplo, bibliotecas a serem usadas, tipo de hardware, etc). Já os
requisitos de sistema adentram em especificações técnicas, e são elaborados pela equipe de desenvolvimento.

Os requisitos podem ainda ser divididos em dois tipos: **funcionais** e **não-funcionais**. Requisitos funcionais
descrevem funcionalidades que o sistema deve ter e como ele deve se comportar, dependendo das entradas que são 
fornecidas. Já os requisitos não-funcionais descrevem **restrições** do sistema. Essa separação não é tão clara assim,
e requisitos não-funcionais de usuário (e.g. "usuários não-logados não devem ser capazes de acessar o sistema") podem 
derivar diversos requisitos funcionais (e.g. "o sistema deve ter uma tela de login").

No desenvolvimento ágil, os requisitos são levantados ao mesmo tempo em que o sistema está sendo desenvolvido, através
de iterações chamadas _sprints_. Já no desenvolvimento usando outros modelos de processo de software, principalmente
para softwares grandes, os requisitos são levantados anteriormente à etapa de desenvolvimento, gerando um documento 
chamado **especificação funcional**. 

## Como é dividida?

Segundo Pressman[^1], a engenharia de requisitos é dividida em sete tarefas: concepção, levantamento, elaboração,
negociação, especificação, validação e gestão.

### 1. Concepção

A concepção é quando percebe-se que será necessário um novo software para resolver um problema existente, ou aproveitar
uma oportunidade de negócio futura.

As necessidades do software concebido podem (e provavelmente irão) mudar no decorrer do andamento do projeto. Porém, é
nesta etapa que a ideia geral do que ele precisa fazer é definida.

Na concepção, definimos "um entendimento básico do problema, as pessoas que querem uma solução, a natureza da solução
desejada e a eficácia da comunicação e colaboração preliminares entre os demais interessados e a equipe de
software"[^1].

### 2. Levantamento

No levantamento, descobre-se quais objetivos o software deve atender, o que deve ser alcançado, como o software irá
atender às necessidades da empresa, e como ele deverá ser usado no dia-a-dia.

Esta etapa parece simples, porém muitas coisas podem dar errado. O **escopo** do software pode ser mal-definido, sendo
definidos detalhes técnicos que mais confundem do que esclarecem; o **entendimento** entre a equipe de desenvolvimento e
os clientes pode não ser dos melhores, com os clientes não sabendo definir exatamente o que gostariam que o software
fizesse, ou então achando que certas coisas são "óbvias", e que portanto não precisam comunicar isto aos
desenvolvedores, por exemplo; e os requisitos podem ser **voláteis**, mudando a todo instante.

### 3. Elaboração

Os requisitos de software são expandidos e refinados, utilizando um modelo de requisitos refinado, que identifica as
funções, comportamento e informações do software.

As interações do usuário com o software são elaboradas e analisadas nesta etapa.

### 4. Negociação

Não é incomum que os clientes peçam mais do que foi originalmente orçado, ou mudem os requisitos que já foram
levantados. Para conciliar isso, é preciso seguir uma estratégia de negociação. Uma boa estratégia é pedir para o
cliente ordenar os requisitos do software de maneira prioritária, colocando os requisitos mais importantes primeiro, e
pedindo para que escolha os que devem ser implementados antes.

### 5. Especificação

Na especificação, materializamos o entendimento dos requisitos do software em um artefato. Este artefato pode ser um
documento de texto, conjunto de diagramas de caso de uso, um protótipo, dentre outros.

### 6. Validação

Na validação, os artefatos produzidos são revisados de acordo com a corretude e qualidade de especificação dos cenários
de uso descritos. A equipe de validação é composta por engenheiros de software, cliente e usuários.

### 7. Gestão de requisitos

O desenvolvimento do software não termina com a entrega do mesmo; é preciso fazer sua manutenção. No decorrer do tempo,
pode ser que novos requisitos sejam elencados, ou antigos sejam alterados. A gestão de requisitos é a etapa que gerencia
como identificar, controlar e acompanhar as necessidades do software no restante da sua vida útil.

[^1]: Pressman. Engenharia de Software: uma abordagem profissional. 7ª edição. 2011. Bookman.  