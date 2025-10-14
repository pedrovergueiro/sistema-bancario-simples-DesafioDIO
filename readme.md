# 💰 Sistema Bancário em Python (Orientado a Objetos)

Este projeto é uma aplicação de **simulação bancária** desenvolvida em **Python**, utilizando conceitos avançados de **Programação Orientada a Objetos (POO)**.  
Permite criar clientes, abrir contas, realizar saques, depósitos e visualizar extratos de forma organizada.

---

## 🚀 Funcionalidades

- Criar clientes (Pessoa Física)
- Criar contas correntes com limite e número máximo de saques
- Realizar **depósitos**
- Realizar **saques**
- Consultar **extrato**
- Listar todas as contas existentes
- Registro automático de todas as transações realizadas

---

## 🧩 Estrutura de Classes

### 🧍‍♂️ `Cliente`
Classe base que representa o cliente, armazena endereço e lista de contas.

### 🧍‍♀️ `PessoaFisica(Cliente)`
Herda de `Cliente`, adicionando informações como nome, CPF e data de nascimento.

### 🏦 `Conta`
Classe base que representa uma conta bancária com métodos para depósito e saque.

### 💳 `ContaCorrente(Conta)`
Herda de `Conta`, adicionando **limite de saque** e **limite de valor** por operação.

### 📜 `Historico`
Armazena todas as transações (data, tipo e valor) realizadas em uma conta.

### 💸 `Transacao` (Classe abstrata)
Modelo base para operações financeiras (Depósito e Saque).

- **`Deposito`**: registra um depósito na conta.
- **`Saque`**: registra um saque na conta.

---

## ⚙️ Estrutura de Arquivos

banco/
├── main.py # Código principal do programa
├── README.md # Documentação do projeto

yaml
Copiar código

---

## 🖥️ Como Executar

1. Certifique-se de ter o **Python 3.8+** instalado.
2. Clone o repositório:

   ```bash
   git clone https://github.com/seu-usuario/nome-do-repositorio.git
   cd nome-do-repositorio
Execute o programa:

bash
Copiar código
python main.py
📋 Menu do Sistema
Ao executar o programa, o menu exibido será:

csharp
Copiar código
================ MENU ================
[1] Depositar
[2] Sacar
[3] Extrato
[4] Nova conta
[5] Listar contas
[6] Novo usuário
[7] Sair
=> 
🧠 Conceitos Aplicados
Programação Orientada a Objetos (POO)

Herança e Polimorfismo

Abstração com classes abstratas

Decoradores (log_transacao)

Iteradores personalizados

Geradores (para extrato filtrado)

Boas práticas e organização modular

🧾 Exemplo de Saída
diff
Copiar código
=== Cliente criado com sucesso! ===
=== Conta criada com sucesso! ===
=== Depósito realizado com sucesso! ===
=== Saque realizado com sucesso! ===

================ EXTRATO ================
Deposito:
    R$ 500.00
Saque:
    R$ 100.00

Saldo:
    R$ 400.00
==========================================
🧑‍💻 Autor
Pedro Lucas Vergueiro Felicio da Silva
📚 Estudante de Engenharia de Software
💡 Foco em desenvolvimento com Inteligência Artificial e Automação

🏷️ Licença
Este projeto é de uso livre para fins educacionais.

yaml
Copiar código

---

Quer que eu gere esse `README.md` pronto para download (com seu nome e repositório já configurados)?  
Posso salvar o arquivo `.md` completo para você baixar direto.