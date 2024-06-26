# Virgo: Desafio técnico para backend

## O desafio

Uma das obrigações que uma securitizadora tem para cumprir é o acompanhamento do fluxo de pagamentos.

1. Imagine que hoje temos um sistema para calcular esses fluxos de pagamentos. O sistema conta com 800 fluxos que precisam ser pagos mensalmente em dias úteis diversos. Hoje o serviço que retorna o fluxo de pagamentos com o valor a ser pago, faz conexão com o banco, vários cálculos e está lento. Em dias específicos há muitos pagamentos e a consulta dos fluxos ficam mais lentos. Na sua visão, como poderíamos iniciar a busca pelo problema, e que tipo de melhoria poderia ser feita? (Não há código aqui. Apenas elabore uma estratégia e compartilhe conosco no nosso papo a ser marcado.)

2. Com base no problema anterior, segue o pedido:
  - Eu como usuário do sistema, gostaria de ter mais controle sobre o fluxo de pagamento.
  - Dado o [sistema de fluxos](#sobre-o-sistema-de-fluxos), quando precisar fazer um pagamento na data prevista, preciso ter um controle de quais pagamentos já foram feitos para fazer somente dos que ainda estão pendentes.
  - Gostaríamos que você codificasse um novo sistema para gerenciar pagamentos feitos e pendentes que chamaria o outro [sistema de fluxos](#sobre-o-sistema-de-fluxos) para obter datas de pagamentos e o valor a ser pago.
  - Na chamada do [sistema de fluxos](#sobre-o-sistema-de-fluxos), simule uma demora de 6s para obter os valores.
  - O controle de pagamentos fica livre à seu critério de como deveria ser a solução.

### Sobre o sistema de fluxos

- adicionamos arquivos para simular uma API que são os arquivos na pasta `api`
- para chamar a API, faça pelo próprio endpiont do GitHub com a url base: `https://raw.githubusercontent.com/virgoinc/job-backend/api`
- para listar os ids dos fluxos: `/fluxos.json`
- para pegar os fluxos com as datas de pagamentos e valores: `/fluxos/:idFluxo`

### O que nós esperamos do seu teste

- O código deverá ser hospedado em algum repositório público. Diversos quesitos serão avaliados aqui, como organização do código, sequencialidade de commits, nomeação de classes e métodos, etc.
- O código deverá estar pronto para ser executado e testado, portanto, caso exista algum requisito, este deve estar completamente documentado no README do seu projeto.
- Marcaremos um papo para você nos explicar a solução e suas motivações.
- Você deverá utilizar a nossa stack de tecnologias: Java ou Kotlin + Spring boot.

### O que nós ficaríamos felizes de ver em seu teste

- Testes
- Processo de build e deploy documentado
- Aplicação rodando pelo Docker

### O que nós não gostaríamos

- Descobrir que não foi você quem fez seu teste
- Ver commits grandes, sem muita explicação nas mensagens em seu repositório

## O que avaliaremos de seu teste

- Histórico de commits do git
- As instruções de como rodar o projeto
- Organização, semântica, estrutura, legibilidade, manutenibilidade do seu código
- Alcance dos objetivos propostos
