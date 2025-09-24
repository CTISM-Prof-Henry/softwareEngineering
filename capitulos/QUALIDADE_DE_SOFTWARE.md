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

### Liberdade de risco

Ao desenvolver um software, para qualquer área de atuação que seja, é importante determinar os riscos que a utilização desse software pode oferecer ao usuário. Softwares com possibilidade de aquisição de itens pagos, como sites de compra e venda, podem oferecer riscos de golpes aos compradores e vendedores, por exemplo. Portanto, durante o desenvolvimento de um software com esse recurso, é necessário pensar em formas de garantir que o comprador vai receber seu produto e o vendedor vai receber seu dinheiro. Porém, além de pensar nos riscos ao usuário, deve-se pensar nos riscos durante o desenvolvimento, como a possibilidade de bugs, invasões ao ambiente de desenvolvimento e o processo de implementação. Durante o desenvolvimento, os seguintes tópicos devem ser pensados cuidadosamente:

1. **Ambiente de desenvolvimento seguro:** o controle e integridade do processo de desenvolvimento deve ficar restrito ao time de desenvolvedores, sem influência externa capaz de executar alguma mudança inesperada no ambiente.
2. **Gestão de código fonte:** contar com uma ferramente de gerenciamento garante maior integridade e organização do código fonte, evitando erros quanto à versão colocada em produção.
3. **Testes e validação:** são etapas necessárias para verificar o comportamento e funcionamento de trechos do código antes da implementação final.
4. **Gestão e correção de bugs:** a documentação e correção dos possíveis bugs é imprescindível para evitar ocorrências semelhantes no futuro.
5. **Integração contínua:** processo que entrega mais qualidade ao software, por automatizar verificações e gerar novos releases.
6. **Documentação do software:** se feita de maneira clara, objetiva e bem estruturada, é uma prática que traz mais qualidade ao processo de desenvolvimento. Isso facilita a ampliação e a melhoria futura.

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

### Portabilidade

A portabilidade de um software se refere a capacidade do mesmo de operar normalmente em outros dispositivos ou softwares. Para medir a portabilidade de um software, deve-se analisar os seguintes aspectos:

1. **Adaptabilidade:** Avalia a capacidade de software de ser adaptado a diferentes plataformas (hardwares ou softwares) sem grandes alterações. Exemplo: Quais alterações são necessárias para que o software funcione corretamente no Windows, MacOS e Android.
2. **Facilidade de instalação:** Mede a simplicidade e a flexibilidade do processo de instalar e desinstalar o software. Exemplo: Quão fácil é a instalação e desinstalação do software em diferentes dispositivos e sistemas.
3. **Capacidade de substituição:** Determina o quão fácil é substituir o software por outro que desempenhe a mesma função. Exemplo: Microsoft Office e LibreOffice realizam as mesmas funções, porém o Microsoft Office se destaca por ser mais completo, possuir integração com outros serviços da empresa, melhor compatibilidade com arquivos de diversos tipos, ser de uma marca muito conhecida, entre outros.
4. **Coexistência:** Refere-se a capacidade do software de compartilhar recursos do sistema sem conflitos com outros softwares. Exemplo: O software deve conseguir funcionar em conjunto com outros softwares do sistema sem causar conflitos, bugs ou falhas no sistema, lentidão ou sobrecarga de uso dos recursos do hardware.

### Como melhorar a portabilidade de um software?

Para melhorar a portabilidade de um software e permitir seu funcionamento em outros hardwares e softwares, é uma boa estratégia criar o software com padrões amplamente aceitos e com suporte em diversas plataformas. A linguagem Java, por exemplo, permite a portabilidade entre sistemas operacionais através do sistema Java Virtual Machines, facilitando a portabilidade. Além disso, reduzir dependências diretas com a plataforma, onde o sistema está sendo desenvolvido, como através de camadas de abstração que desacoplam o código das especificidades do sistema operacional. Por fim, é muito importante realizar testes do software em diferentes plataformas durante o processo de desenvolvimento, para identificar problemas de portabilidade desde o início.

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
