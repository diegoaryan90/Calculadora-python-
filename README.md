# Calculadora-python-
Sou iniciante, e esse é o meu primeiro projeto.
def calculadora():
    while True:
        print("Operações:")
        print("1. Soma")
        print("2. Subtração")
        print("3. Multiplicação")
        print("4. Divisão")
        print("5. Sair")

        escolha = input("Escolha uma opção: ")

        if escolha == "5":
            break

        elif escolha not in ["1", "2", "3", "4"]:
            print("Opção inválida. Tente novamente!")
            continue

        num1 = float(input("Digite o primeiro número: "))
        num2 = float(input("Digite o segundo número: "))

        if escolha == "1":
            resultado = num1 + num2
            print(f"{num1} + {num2} = {resultado}")

        elif escolha == "2":
            resultado = num1 - num2
            print(f"{num1} - {num2} = {resultado}")

        elif escolha == "3":
            resultado = num1 * num2
            print(f"{num1} * {num2} = {resultado}")

        elif escolha == "4":
            if num2 != 0:
                resultado = num1 / num2
                print(f"{num1} / {num2} = {resultado}")
            else:
                print("Erro: divisão por zero!")

calculadora()
