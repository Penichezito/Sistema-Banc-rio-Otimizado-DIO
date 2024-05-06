# Sistema Bancário 2 [Otimizado]

Este é um sistema bancário simples que permite realizar operações como depósito, saque, exibição de extrato, criação de usuários e contas. Vou explicar cada parte do código.

Função menu()
A função menu() exibe um menu de opções para o usuário. Ele pode escolher entre as seguintes opções:

[d] Depositar
[s] Sacar
[e] Extrato
[nc] Nova Consulta
[lc] Listar contas
[nu] Novo usuário
[q] Sair
Função depositar(saldo, valor, extrato)
Esta função permite fazer um depósito. Ela verifica se o valor informado é válido (maior que zero) e atualiza o saldo e o extrato.

Função sacar(saldo, valor, extrato, limite, numero_saques, limite_saques)
A função sacar() permite fazer um saque. Ela verifica se o valor do saque não excede o saldo, o limite ou o número máximo de saques permitidos. Se tudo estiver correto, ela atualiza o saldo e o extrato.

Função exibir_extrato(saldo, extrato)
Essa função exibe o extrato bancário, mostrando todas as movimentações realizadas e o saldo atual.

Função criar_usuario(usuarios)
A função criar_usuario() permite criar um novo usuário. Ela solicita o CPF, verifica se já existe um usuário com esse CPF e, se não existir, coleta informações como nome, data de nascimento e endereço para criar o usuário.

Função filtrar_usuario(cpf, usuarios)
Essa função filtra os usuários com base no CPF fornecido. Se encontrar um usuário com o CPF especificado, retorna esse usuário; caso contrário, retorna None.

Função criar_conta(agencia, numero_conta, usuarios)
A função criar_conta() permite criar uma nova conta. Ela solicita o CPF do usuário, verifica se o usuário existe e, se sim, cria uma nova conta associada a esse usuário.

Função listar_contas(contas)
Essa função lista todas as contas existentes, exibindo informações como agência, número da conta e titular.

Função main()
A função main() é o ponto de entrada do programa. Ela define algumas constantes (como o limite de saques e a agência), inicializa variáveis e entra em um loop para processar as opções do usuário.
