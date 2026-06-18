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

### Eficácia
#### Objetivo do Software
Garantir que os usuários consigam agendar salas de forma rápida, eficiente e sem conflitos, atendendo às necessidades do negócio.

---

# Avaliação de Sistema de Agendamento de Salas

## 1. Testes Funcionais (máx. 4 pontos)

Verifica se as funcionalidades principais estão operando corretamente:

| Funcionalidade                | Descrição                                                                 | Resultado Esperado                             | Pontuação |
|------------------------------|---------------------------------------------------------------------------|------------------------------------------------|-----------|
| Criar Agendamento            | Agendar sala em data/hora disponível                                      | Deve agendar com sucesso                       | 1         |
| Evitar Conflitos de Horário  | Impedir dois usuários de agendarem a mesma sala no mesmo horário          | Sistema deve bloquear o segundo agendamento    | 1         |
| Cancelar Agendamento         | Cancelar uma reserva previamente criada                                   | Sistema deve liberar o horário corretamente    | 1         |
| Visualizar Agenda            | Consultar a agenda da sala                                                | Sistema deve exibir horários ocupados e livres | 1         |

**Total Testes Funcionais:** _/4_

---

## 2. Testes de Aceitação com Usuários Finais (máx. 1 ponto)

Realizados com usuários reais, simulando situações do dia a dia:

- Agendar reuniões
- Cancelar ou alterar reservas
- Buscar salas disponíveis

**Critério de sucesso:** A maioria dos usuários utiliza o sistema com facilidade e considera que ele atende às necessidades.

**Pontuação:** _/1_

---

## 3. Teste de Validação de Sistema (máx. 1 ponto)

Verifica se o sistema funciona de ponta a ponta, com todos os componentes integrados:

**Fluxo Validado:**
1. Login do usuário
2. Agendamento da sala
3. Envio de e-mail automático aos participantes
4. Bloqueio do horário agendado

**Critério de sucesso:** Todo o fluxo deve funcionar sem falhas.

**Pontuação:** _/1_

---

## 4. Análise dos Resultados (máx. 1 ponto)

Avaliação geral baseada nos testes anteriores:

- Funcionalidades passaram ou falharam?
- Conflitos de agendamento foram evitados?
- Usuários conseguiram realizar suas tarefas?

**Critério de sucesso:** O sistema atendeu aos objetivos e requisitos definidos no início do projeto.

**Pontuação:** _/1_

---

## 5. Feedback dos Usuários (máx. 1 ponto)

Coleta de opiniões dos usuários (via formulários simples):

- Facilidade de uso
- Clareza da interface
- Eficiência geral
- Satisfação

**Critério de sucesso:** Feedback positivo na maioria dos aspectos avaliados.

**Pontuação:** _/1_

---

## 6. Teste de Desempenho (máx. 1 ponto)

Avalia a resposta do sistema sob carga:

- Vários usuários simultâneos
- Múltiplos agendamentos sendo processados

**Critério de sucesso:** Sistema responde bem e sem lentidão em situações com carga elevada.

**Pontuação:** _/1_

---

## 7. Documentação das Descobertas (máx. 1 ponto)

Verifica se foram registrados:

- Erros encontrados
- Ajustes realizados
- Pontos de melhoria

**Critério de sucesso:** A documentação está clara e completa.

**Pontuação:** _/1_

---

## Avaliação Final – Sistema de Score

| Critério                          | Pontos Máximos | Pontos Obtidos |
|----------------------------------|----------------|----------------|
| Testes Funcionais                | 4              |                |
| Testes de Aceitação              | 1              |                |
| Teste de Validação de Sistema    | 1              |                |
| Teste de Desempenho              | 1              |                |
| Análise dos Resultados           | 1              |                |
| Documentação das Descobertas     | 1              |                |
| Feedback dos Usuários            | 1              |                |
| **Total**                        | **10**         |                |

---

## Interpretação do Score

| Pontuação Total | Nível de Eficácia                      |
|-----------------|----------------------------------------|
| 9 a 10          | Software altamente eficaz           |
| 7 a 8           | Eficaz, com pequenas melhorias       |
| 5 a 6           | Funcional, mas com melhorias a fazer |
| Abaixo de 5     | Pouco eficaz, precisa de revisão     |

---

## Conclusão

Um sistema de agendamento de salas é considerado **eficaz** quando:

- Atende aos requisitos funcionais e de negócio
- Evita conflitos e erros de agendamento
- Funciona corretamente mesmo com uso intenso
- Recebe boa aceitação dos usuários

---



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

---

## Manutenibilidade

Garantir que o sistema seja fácil de modificar, corrigir, evoluir e manter ao longo do tempo, reduzindo custos e evitando deterioração do código.

---

### Objetivo da Manutenibilidade
Facilitar a compreensão, alteração e evolução do sistema com baixo esforço e alta qualidade, promovendo código claro, consistente e bem documentado.

---

### Métricas para Avaliação da Manutenibilidade

---

#### Legibilidade  
**O que avaliar:** Quão fácil é para desenvolvedores, de diferentes níveis, entenderem o código.  
**Como medir:** Linter
**Meta:** 80% ou mais de aprovação  

---

#### Consistência  
**O que avaliar:** Adoção de convenções e padrões no código.  
**Como medir:** Linter
**Meta:** 80% ou mais de aprovação.  

---

#### Clareza  
**O que avaliar:** Complexidade das estruturas de controle (if-else, loops, etc).  
**Como medir:** Linter
**Meta:** 80% ou mais de aprovação
---

#### Baixo Acoplamento  
**O que avaliar:** Dependências entre módulos e funções.  
**Como medir:** Número de chamadas cruzadas entre módulos/funções.  
**Critério:** Módulos independentes, com poucas interdependências.  

---

#### Alta Coesão  
**O que avaliar:** Foco das funções e classes em uma única responsabilidade.  
**Como medir:** Linter
**Meta:** 80% ou mais de aprovação

---

#### Documentação Eficaz  
**O que avaliar:** Presença e qualidade dos comentários e documentação interna.  
**Como medir:** Linter
**Meta:** 80% ou mais de aprovação
---

#### Simplicidade  
**O que avaliar:** Tamanho e complexidade das funções/métodos.  
**Como medir:** Linter
**Meta:** 80% ou mais de aprovação
---

##### Testes Contínuos  
**O que avaliar:** Cobertura e frequência de testes automatizados.  
**Como medir:** Linter
**Meta:** 80% ou mais de aprovação

---

#### Análise dos Resultados  
Após avaliação, registre:  

- Pontos fortes da manutenibilidade.  
- Áreas que precisam de melhoria (ex: aumentar documentação, reduzir acoplamento).  
- Recomendações para próximas versões ou refatorações.

---

#### Documentação das Descobertas  
Elabore um relatório com:  

- Descrição dos testes e avaliações realizados.  
- Resultados quantitativos (scores).  
- Exemplos de trechos de código para ilustrar problemas ou bons exemplos.  
- Sugestões práticas para melhorias.

---

#### Conclusão  
Um sistema com boa manutenibilidade é aquele que apresenta:  

- Código fácil de entender e modificar.  
- Baixo acoplamento e alta coesão.  
- Documentação clara e atualizada.  
- Cobertura adequada de testes automatizados.  



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
