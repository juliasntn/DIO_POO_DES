# ESSE E UM DESAFIO DA DIO

# Sistema Bancário

Este é um sistema bancário simples implementado em Python, que permite a criação de clientes, contas correntes, e a realização de transações como depósitos e saques. O sistema também exibe o extrato das contas e lista todas as contas existentes.

## Funcionalidades

- **Criar Cliente**: Permite a criação de novos clientes com nome, CPF, data de nascimento e endereço.
- **Criar Conta Corrente**: Permite a criação de contas correntes associadas a clientes existentes.
- **Depositar**: Realiza depósitos em contas correntes.
- **Sacar**: Realiza saques em contas correntes, respeitando limites e número de saques permitidos.
- **Exibir Extrato**: Exibe o extrato de uma conta corrente, mostrando todas as transações realizadas.
- **Listar Contas**: Lista todas as contas correntes existentes no sistema.

## Estrutura do Código

### Classes Principais

- **Cliente**: Representa um cliente do banco, contendo informações como endereço e contas associadas.
- **PessoaFisica**: Subclasse de Cliente, adiciona informações específicas de pessoas físicas como nome, data de nascimento e CPF.
- **Conta**: Representa uma conta bancária, contendo saldo, número, agência, cliente associado e histórico de transações.
- **ContaCorrente**: Subclasse de Conta, adiciona funcionalidades específicas de contas correntes como limite e limite de saques.
- **Historico**: Mantém o histórico de transações realizadas em uma conta.
- **Transacao**: Classe abstrata para representar uma transação bancária.
  - **Saque**: Subclasse de Transacao, representa uma operação de saque.
  - **Deposito**: Subclasse de Transacao, representa uma operação de depósito.

### Funções Principais

- **menu**: Exibe o menu principal e captura a escolha do usuário.
- **filtrar_cliente**: Filtra clientes pelo CPF.
- **recuperar_conta_cliente**: Recupera a conta de um cliente.
- **depositar**: Realiza a operação de depósito.
- **sacar**: Realiza a operação de saque.
- **exibir_extrato**: Exibe o extrato de uma conta.
- **criar_cliente**: Cria um novo cliente.
- **criar_conta**: Cria uma nova conta corrente.
- **listar_contas**: Lista todas as contas existentes.
- **main**: Função principal que executa o loop do menu.

## Como Executar

1. Clone o repositório:

   ```sh
   git clone https://github.com/seu-usuario/sistema-bancario.git
   cd sistema-bancario
   ```

2. Execute o script Python:

   ```sh
   python nome_do_arquivo.py
   ```

## Exemplo de Uso

Ao executar o script, você verá um menu com as opções:

```
=============== MENU ================
[d] Depositar
[s] Sacar
[e] Extrato
[nc] Nova conta
[lc] Listar contas
[nu] Novo usuário
[q] Sair
=>
```

Siga as instruções exibidas para realizar as operações desejadas.

## Contribuição

Se você quiser contribuir com este projeto, por favor siga estas etapas:

1. Faça um fork do repositório.
2. Crie uma branch para sua feature (`git checkout -b feature/nome-da-feature`).
3. Commit suas alterações (`git commit -am 'Adiciona nova feature'`).
4. Faça push para a branch (`git push origin feature/nome-da-feature`).
5. Abra um Pull Request.

## Contato

E-mail: falecomjuliasantana@gmail.com
