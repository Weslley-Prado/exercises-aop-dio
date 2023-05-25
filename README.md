# Projeto de Sistema Bancário

Este é um projeto de exemplo que implementa um sistema bancário básico usando o paradigma de programação orientado a objetos. O objetivo é demonstrar a estrutura e funcionalidades das classes relacionadas a contas bancárias.

## Classes

### Classe `Conta`

A classe `Conta` representa uma conta bancária genérica e possui os seguintes atributos:

- `TipoConta`: o tipo de conta (corrente, poupança, investimento, etc.).
- `TipoCliente`: o tipo de cliente associado à conta.
- `DataAbertura`: a data de abertura da conta.
- `Saldo`: o saldo atual da conta.

A classe `Conta` possui os seguintes métodos:

- `sacar(valor)`: realiza um saque na conta, diminuindo o saldo pelo valor especificado.
- `depositar(valor)`: realiza um depósito na conta, aumentando o saldo pelo valor especificado.
- `calcularValorTarifaManutencao()`: calcula o valor da tarifa de manutenção da conta.

### Classe `ContaPoupanca`

A classe `ContaPoupanca` é uma subclasse de `Conta` e adiciona a funcionalidade específica de uma conta poupança. Não possui atributos adicionais.

A classe `ContaPoupanca` sobrescreve o método `calcularValorTarifaManutencao()` para calcular o valor da tarifa de manutenção de uma conta poupança.

### Classe `ContaInvestimento`

A classe `ContaInvestimento` é uma subclasse de `Conta` e adiciona a funcionalidade específica de uma conta de investimento. Não possui atributos adicionais.

A classe `ContaInvestimento` sobrescreve o método `calcularValorTarifaManutencao()` para calcular o valor da tarifa de manutenção de uma conta de investimento.

## Aspecto de Verificação de Saldo

O projeto também inclui um aspecto chamado `VerificacaoSaldoAspect` implementado usando a extensão de linguagem AspectJ. Esse aspecto é responsável por verificar o saldo em todas as contas antes de permitir um saque.

O aspecto `VerificacaoSaldoAspect` contém a lógica para verificar o saldo em todas as contas e exibir uma mensagem de saldo insuficiente, se necessário.

## Observações

- O projeto foi desenvolvido em Java e utiliza a extensão AspectJ para implementar o aspecto.
- Este é um exemplo básico para fins de demonstração e pode ser expandido de acordo com os requisitos específicos do sistema bancário.

Esse é apenas um exemplo básico de como você pode escrever um README para documentar as classes do seu projeto. Sinta-se à vontade para adicionar mais detalhes, como informações sobre como compilar e executar o projeto, outras funcionalidades, entre outros, conforme necessário.
