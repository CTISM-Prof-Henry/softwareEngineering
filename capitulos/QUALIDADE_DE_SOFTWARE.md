# Qualidade de Software

A qualidade de software é definida pela família ISO 25000 de normas e diz respeito a aspectos que mensuram a qualidade 
de um software sob a vista de duas grandes áreas: qualidade de uso e qualidade do produto.

A ISO 25000 define o modelo **SQuaRE: Software Quality Requirements and Evaluation** (Requisitos e Avaliação da 
Qualidade do Software).

## Uma nota sobre história e normas

Quando você estudar sobre modelos de qualidade, talvez você encontre material sobre a ISO 9126. Esta ISO foi proposta 
em 1991 e revisada em 2001. Posteriormente, foi substituída pela ISO 25000, que segue (até pelo menos o ano de 2025) 
sendo a norma vigente sobre qualidade de software.

Além disso, qual o relacionamento entre a ISO 25000 e 25010? É importante ter em mente que a Organização Internacional
de Normalização (International Standardization Organization -- ISO) propõe normas **gerais** e **específicas**. 
Enquanto a ISO 25000 é o guia geral da família SQuaRE, a ISO 25010 trata especificamente das maneiras de categorizar
e mensurar os aspectos de qualidade, sendo o modelo de qualidade propriamente.

## Qualidade de Uso

É subdividida em 5 categorias, definidas pela ISO 25010:

1. **Eficácia:** o software cumpre os objetivos? 
2. **Eficiência:** O software atende os requisitos exigindo pouco esforço do usuário para sua manipulação?
3. **Satisfação:** O usuário ficou satisfeito?
4. **Liberdade de risco:** O software, ao ser usado, oferece riscos à integridade do usuário?
5. **Cobertura de contexto:** O software funciona sob diferentes condições de uso?


<img alt="escavadeira" src="../imagens/escavadeira.webp" width="400px">

### Eficiência

A eficiência relaciona-se ao uso otimizado dos recursos disponíveis pelo software, incluindo tempo (velocidade). Nesse sentido, um sistema eficiente deve realizar suas funções rapidamente e facilmente pelo usuário.

Softwares eficientes melhoram a experiência geral do usuário ao reduzir o tempo que o usuário demora para realizar ações ao aumentar a responsividade das aplicações.

Exemplo: Aplicativo de Banco, um cliente usa o app para transferir dinheiro.
Será ineficiênte se o usuário demorar muito tempo para descobrir como fazer a transferência.  
Será eficiênte se o aplicativo for intuitivo nas funcionalidades, conseguir fazer a transferência em poucos segundos e em poucos toques.
Nesse exemplo a métrica da boa eficiência é o tempo, medido por quantos segundos o usuário demora para realizar a ação utilizando as funcionalidades do sistema.

Exemplo: Sistema de gestão empresárial, um funcionário precisam gerar relatórios mensais urgente por conta que o chefe pediu.
Será ineficiênte se o usuário não conseguir gerar os relatórios no prazo que o chefe pediu por conta da interface não intuitiva do app.
Será eficiênte se o sistema gerar o mesmo relatório em poucos cliques, em pouco tempo e quando o usuário precisar/quiser.
Nesse exemplo a métrica da boa eficiência é o tempo, medido por quantos segundos o usuário demora para realizar a ação utilizando as funcionalidades do sistema.

## Qualidade do Produto

Novamente, é subdividida em oito categorias, definidas pela ISO 25010:

1. **Compatibilidade:** capacidade de coexistir ou interagir com outros sistemas.
2. **Segurança:** proteção de dados e controle de acesso.
3. **Adequação funcional:** cobertura e correção das funções.
4. **Confiabilidade:** disponibilidade, tolerância a falhas, etc
5. **Usabilidade:** facilidade de aprendizado e operação.
6. **Eficiência de Desempenho:** tempo de resposta, uso de recursos.
7. **Manutenibilidade:** facilidade de modificar, corrigir, evoluir.
8. **Portabilidade:** capacidade de ser transferido para outros ambientes.

<img alt="relógio de luxo" src="../imagens/patek_philippe.png" width="400px">

### Adequação Funcional

Esta característica representa o grau em que um produto ou sistema fornece funções que atendem às necessidades declaradas e implícitas quando utilizado sob condições especificadas. Esta característica é composta pelas seguintes subcaracterísticas:

Completude funcional - Grau em que o conjunto de funções abrange todas as tarefas especificadas e os objetivos dos usuários pretendidos.
Correção funcional - Grau em que um produto ou sistema fornece resultados precisos quando utilizado pelos usuários pretendidos.
Adequação funcional - Grau em que as funções facilitam a realização de tarefas e objetivos especificados.

Exemplo: Sistema E-commerce, o software é capaz de calcular o frete de forma precisa em todos os pedidos sem erro.
Exemplo: Aplicativo de rede social, deve permitir que os usuários criem seus perfis, editem informações pessoais e interajam com outros usuários conforme definido nos requisitos.

## Como mensurar a qualidade?

A maneira de mensurar qualidade depende do que a equipe de desenvolvimento definir junto com o cliente. Não existem critérios rígidos, e 
diferentes métricas podem ser adotadas.

Os passos para mensurar a qualidade são os seguintes:

1. Elencar quais itens da qualidade de uso e qualidade do produto são importantes para o software em questão. Nem todo
   software possuirá os mesmos requisitos!
2. Escolher uma ou mais métricas para cada um dos itens selecionados. 
3. Definir como essas métricas serão medidas e coletadas.
4. Definir a meta. Por exemplo:
   * A categoria é **portabilidade**
   * A métrica é **número de versões de Android suportadas pelo software**
   * A meta é **as últimas 5 versões**

## Bibliografia

* [ISO 25010](https://iso25000.com/index.php/en/iso-25000-standards/iso-25010)
