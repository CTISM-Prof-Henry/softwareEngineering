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
