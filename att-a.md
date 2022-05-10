# questaoa

nconsumidor = input("Qual o número de cadastro?")    #Pergunta qual o número de cadastro do usuário
kwhdia = input("Qual a quantidade de kWh consumida no dia?")    #Pergunta qual a quantidade de KWh consumidos no dia
codigoconsumidor = int(input("Em qual consumidor você se enquadra?\n1 - Residencial, 2 - Comercial, 3 - Industrial\n"))   #Pergunta em qual consumidor o usuário se enquadra

#Informa o custo de KWh consumido
if codigoconsumidor == 1:    
    print("Custo total:")   
    print(float(kwhdia) * float(0.3))          
if codigoconsumidor == 2:
    print("Custo total:")
    print(float(kwhdia) * float(0.5))    
elif codigoconsumidor == 3:
    print("Custo total:")
    print(float(kwhdia) * float(0.7))
    
#Informa a média do consumidor tipo 1 e 2
print("A média de consumo entre os consumidored 1 e 2 é:" , (float(kwhdia) * float(0.3) + float(kwhdia) * float(0.5)/2))
