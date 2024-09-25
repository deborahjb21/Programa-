# Programa para calcular se um número pertence à sequência de Fibonacci (em Python):
def is_fibonacci(num):
    a, b = 0, 1
    while b <= num:
        if b == num:
            return True
        a, b = b, a + b
    return False
# Entrada do número
numero = int(input("Informe um número: "))
# Verificação se o número pertence à sequência
if is_fibonacci(numero):
    print(f"O número {numero} pertence à sequência de Fibonacci.")
else:
    print(f"O número {numero} NÃO pertence à sequência de Fibonacci.")
