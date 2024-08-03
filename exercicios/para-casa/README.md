# Exercício de Casa 🏠 

### Objetivos de aprendizagem do desafio 🎯

- Aprender sobre a importância e os benefícios dos testes  em desenvolvimento de software.
- Compreender a diferença entre testes unitários, testes de integração e testes end-to-end (E2E).
- Aplicar a metodologia TDD (Test-Driven Development) no desenvolvimento de novas funcionalidades.
- Escrever testes unitários utilizando frameworks de teste em TypeScript.
- Criar testes de integração para validar a interação entre diferentes partes do sistema.
- Desenvolver testes end-to-end para garantir que o fluxo completo do usuário funcione conforme esperado.

<h2 align=center> {Reprograma}Bank </h2>
  <h3>Implementando Testes e TDD</h3>

Seu desafio é implementar testes  para o sistema bancário desenvolvido nas semanas anteriores. Como desafio extra, você deverá utilizar a metodologia TDD para criar novas funcionalidades, como a função de Cartão de Crédito.

Abaixo estão os requisitos:

- Escrever testes unitários para todas as classes criadas até agora (Cliente, Gerente, Conta, ContaCorrente, ContaPoupanca).
- Criar testes de integração para a API, verificando a interação entre os diferentes endpoints.
- Desenvolver testes end-to-end para garantir que o fluxo completo do usuário funcione corretamente (exemplo: criação de cliente, abertura de conta, realização de transferência).

#### Desafio Extra
Para aquelas que querem se desafiar, fica aqui a feature de Cartão de Crédito. Ela possui várias regras, implemente as que você conseguir.

- Utilizar TDD para implementar a funcionalidade de cartão de crédito.
- Regras de negocio:
    - Todos os clientes com Conta Corrente agora podem possuir cartão de crédito com o limite inicial de 500 reais com data de fechamento de fatura todo ultimo dia do mes vigente
    - Cartão de Credito possui numero, validade, codigo verificador e bandeira 
    - Cartão de crédito tem a função de transaçao de compra que recebe dados do cartão, data, valor e CNPJ da empresa que vai receber o pagamento
    - A cada compra o limite do mes deve ser diminuido, se a compra for menor que o limite atual, retorne uma mensagem de erro.
    - A fatura deve conter a somatória dos valores feitos no mês do dia primeiro até o ultimo dia do mes
    - Cartão de crédito possui a rota de pagamento de fatura, que debita do salto de conta corrente
    - A cada pagamento completo do valor de fatura o limite deve ser restabelecido
    - Não é possivel fazer parcelamento
    - Não existe extrato das transações de cartão
    - Vamos imaginar que todo cliente vai sempre pagar em dia e que ele sempre vai possuir saldo para pagamento
