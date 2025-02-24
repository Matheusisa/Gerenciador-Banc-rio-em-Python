# Gerenciador Bancário em Python

## Descrição
Este é um sistema bancário simples desenvolvido em **Python** que permite a criação e gerenciamento de contas bancárias, permitindo operações como **depósito, saque e extrato**. O sistema também permite o **cadastro de clientes e contas correntes**, além de manter um histórico de transações.

## Tecnologias Utilizadas
- **Linguagem:** Python 3
- **Paradigma:** Programação Orientada a Objetos (POO)
- **Bibliotecas:** Nenhuma biblioteca externa é necessária para rodar o código

## Funcionalidades
- Criar clientes
- Criar contas correntes
- Realizar depósitos e saques
- Exibir extrato bancário
- Listar contas cadastradas
- Controlar limites de saque
- Manter histórico de transações

## Estrutura do Código
O sistema segue uma estrutura baseada em classes:

### 1. **Cliente e Pessoa Física**
- `Cliente`: Classe base que armazena o **endereço** e as **contas** do cliente.
- `PessoaFisica`: Subclasse de `Cliente`, adiciona os atributos **nome, CPF e data de nascimento**.

### 2. **Conta e Conta Corrente**
- `Conta`: Classe base que gerencia **saldo, número, agência, cliente e histórico de transações**.
- `ContaCorrente`: Subclasse de `Conta`, implementa **limite de saque** e **limite diário de saques**.

### 3. **Transações**
- `Transacao`: Classe abstrata para operações bancárias.
- `Saque`: Implementa a operação de **saque**, verificando limites antes de autorizar.
- `Deposito`: Implementa a operação de **depósito**.

### 4. **Histórico de Transações**
- `Historico`: Armazena todas as transações realizadas em uma conta.

### 5. **Interface do Usuário (menu interativo)**
O sistema possui uma interface de **linha de comando (CLI)** onde o usuário pode escolher ações como **depósito, saque, extrato e criação de conta** através de entradas no teclado.

## Como Executar o Programa

### 1. Requisitos
- Ter o **Python 3** instalado no sistema.

### 2. Executar o script
Salve o código-fonte em um arquivo chamado `banco.py` e execute o seguinte comando no terminal:

```bash
python banco.py
```

### 3. Utilização do Menu
Ao executar o script, será exibido um menu com as seguintes opções:

```
=============== MENU ================
[d]  Depositar
[s]  Sacar
[e]  Extrato
[nc] Nova conta
[lc] Listar contas
[nu] Novo usuário
[q]  Sair
```

Escolha uma opção e siga as instruções na tela.

## Exemplo de Uso
1. Criar um novo cliente (`nu`)
2. Criar uma conta para esse cliente (`nc`)
3. Realizar um depósito (`d`)
4. Fazer um saque (`s`)
5. Consultar extrato (`e`)
6. Listar contas (`lc`)
7. Sair do programa (`q`)

## Melhorias Futuras
- Permitir que o cliente escolha entre múltiplas contas
- Implementação de uma interface gráfica
- Persistência de dados utilizando banco de dados


