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
4. **Satisfação:** O usuário ficou satisfeito?
5. **Liberdade de risco:** O software, ao ser usado, oferece riscos à integridade do usuário?
6. **Cobertura de contexto:** O software funciona sob diferentes condições de uso?


<img alt="escavadeira" src="../imagens/escavadeira.webp" width="400px">

## Eficácia

DESCRIÇÃO:
sobre o assunto eficácia temos métricas para medir o quanto um software cumpre bem seus objetivos
Por exemplo temos uma aplicação de padaria com sistema de estoque e emissão de nota fiscal
- [ ] Emissão de nota fiscal
A emissão de nota fiscal é um requisito funcional para a padaria

como avaliar a eficácia?
1. testar o processo de emissão de uma nota fiscal, verificando se ela está cumprindo com todas as exigências legais, se ela
é rápida sem erros(como a emissão de cpf).
2. testar a validação do envio das notas para o governo e para o sistema do governo

- [ ] Gestão de estoque
      A gestão de estoque é outro requisito funcional pois a padaria precisa garantir que não falte produtos disponiveis para a venda
      
como avaliar a eficácia?
1. verificar se o sistema registra todas as transações de entradas e saídas de produto
2. testar a emissão de relatórios das transações de entradas e saídas(sem erros)



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

## Segurança

Para avaliar a qualidade da segurança do produto é necessário avaliar os seguintes critérios

- [ ] Confidencialidade - Garantir a segurança dos dados
- [ ] Integridade - Grau em que um sistema, produto ou componente garante que o estado de seu sistema e dados esteja protegido
      contra modificações ou exclusões não autorizadas, seja por ação maliciosa ou erro de computador.
- [ ] Não-repúdio - Grau em que ações ou eventos podem ser provados como tendo ocorrido, de modo que não possam ser negados posteriormente.
- [ ] Responsabilidade - Capacidade de rastrear ações de uma entidade
- [ ] Autenticidade - Grau em que a identidade de um sujeito ou recurso pode ser comprovada como sendo a alegada.
- [ ] Resistência - Capacidade do sistema manter sua operação enquanto está sob ataque de um agente malicioso.

Como testar?

Pergunta: Apenas pessoas autorizadas conseguem acessar o sistema da padaria?
O sistema tem controle de acesso com usuários e senhas?
Os dados do estoque, preços e notas fiscais estão restritos a funcionários com permissão (ex: só o gerente pode editar preços)?
Existe criptografia nos dados sensíveis (como CPF/CNPJ de clientes ou informações fiscais)?

Pergunta: Os dados de estoque e notas fiscais permanecem corretos e íntegros ao longo do tempo?
O sistema registra corretamente a entrada e saída de produtos do estoque?
Há validação contra erros ou manipulações (por exemplo, impedir que se registre a venda de produtos inexistentes)?
O sistema evita a modificação de notas fiscais emitidas?

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
