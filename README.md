#Itens de uma pizzaria/esfiharia. Cliete faz os pedidos e então ele tem a contagem do total de esfihas, levando a uma promoção.
#Para o executar o arquivo em .sh basta colocar o "./" antes do nome do arquivo.(Exemplo: ./meu_primeiro_script.sh

#Caso tenha 3 pizzas e um refrigerante, 10% de desconto/Caso tenha mais de 40 esfihas e um refrigerante, 10% de desconto

#Caso tenha 3 pizzas, 40 esfihas e 2 refrigerantes 15% de desconto(combo saidinha da igreja)

esfihas = ["queijo", "carne", "calabresa", "pizza", "bauru"]
pizzas = ["SaborPizza", "Mussarela", "QueijoBranco, GoiabadaM&M", "ChocolateVerdadeiro"]
refrigerante = ["Coca-Cola Lilith", "Soda Samael", "Sprite Aun Weor", "Guaraná Jesus", "Guaraná Diabo"]


print("Somos a Pizzaria e Esfiharia 'Meu Primeiro Algoritmo', vem vindo que já estamos aqui com o melhor de SP..:PS, não atendemos cariocas")
input("Cara hoje o dia tá pra esfiha. Passou na TV. Juro, menzinhô! E ai, vamo de umas 30? \n")

total_esfihas = []

for esfiha in esfihas:
   print("Estas são nossas esfihas: ")
   quantidade_esfihas = int(input(f"Diz pra gente quantas esfihas você deseja: {esfiha} "))
   total_esfihas.append(quantidade_esfihas)

print("Confira se tá tudo como você pediu: ", total_esfihas)

print(" Ficaram um total de: ", sum(total_esfihas))

print("Vamo de pizzinha?")

total_pizzas = []

for pizza in pizzas:
  print("Estas são as pizzas da casa: ")
  quantidade_pizzas = int(input(f"Fala pra nóis quantas você quer dessa: {pizza} "))
  total_pizzas.append(quantidade_pizzas)

print("Que pedido top!")

print("Boato que são as melhores daqui, mas fica entre nós. Confirma se tá certo na maciota: ", sum(total_pizzas), "pizzas")

str(input("Vai um refri?: "))

total_bebidas = []

for bebidas in refrigerante:
   print("Esses são nossos refris disponíveis: ")
   quantidade_bebidas = int(input(f"Vai querer qual: {bebidas} "))
   total_bebidas.append(quantidade_bebidas)

print("Foram esses mata-sede, mesmo?: ", sum(total_bebidas))

input("Pedido feito, meu chapa!")
