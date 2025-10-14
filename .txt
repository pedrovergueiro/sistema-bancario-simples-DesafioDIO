menu = '''

[1] saque
[2] deposito
[3] extrato
[4] sair

'''

saldo = 0
limite = 500
limite_saque = 3
extrato = ''
numero_de_saques = 0

while True:

    opcao = input(menu)

    if opcao == '1':
        valor = float(input('informe o valor do saque: '))
        excedeu_saldo = valor > saldo
        excedeu_limite = valor > limite
        excedeu_saque = numero_de_saques >= limite_saque

        if excedeu_saldo:
            print('Saldo insuficiente.')

        elif excedeu_limite:
            print('O valor do saque excede o limite permitido.')

        elif excedeu_saque:
            print('Você excedeu o limite de 3 saques diários.')

        else:
            saldo -= valor
            extrato += f'Saque: R${valor:.2f}\n'
            numero_de_saques += 1
            print('Saque realizado com sucesso!')

    elif opcao == '2':
        valor = float(input('digite o valor do deposito: '))

        if valor > 0:
            saldo += valor
            extrato += f'Deposito: R${valor:.2f}\n'
            print('Depósito realizado com sucesso!')
        else:
            print('Operação falhou: valor inválido.')

    elif opcao == '3':
        print('\n========== EXTRATO ==========')
        print('Nenhuma movimentação.' if extrato == '' else extrato)
        print(f'Saldo atual: R${saldo:.2f}')
        print('=============================\n')

    elif opcao == '4':
        print('Saindo...')
        break

    else:
        print('Opção inválida, tente novamente.')
