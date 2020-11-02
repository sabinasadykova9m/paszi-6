# paszi-6
alphabet = [chr(i) for i in range(ord('а'), ord('я')+1)]
word = input("Введите слово, которое хотите зашифровать:")
massiv=[]
result = [alphabet.index(i) + 1 for i in word]
print(result)
a=int(input("a="))
p=int(input("p="))
for i in range(len(result)):
    if (1<=result[i]<=p-1) and (1<=a<=p):
        massiv.append(a**result[i]%p)
    else:
        print("Ошибка")
print(massiv)
