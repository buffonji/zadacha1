# zadacha3
def is_prime(num):
    if num < 2:
        return False
    for i in range(2, int(num**0.5) + 1):
        if num % i == 0:
            return False
    return True

start = 47584
end = 47684
primes = []

# Ищем простые числа
for number in range(start, end + 1):
    if is_prime(number):
        primes.append(number)

# Выводим результаты
for index, prime in enumerate(primes, start=1):
    print(index, prime)
