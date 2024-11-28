##Buenos Dias- Tardes - Noches 👋

--> # Segunda entrega
# Definición de variables (reemplaza los valores con los que te proporcionen)
V = 100  # Número de vacas
A = 200  # Número de aves
K = 5   # Metros cuadrados de pasto por vaca
X = 10  # Litros de leche por vaca por día

# problema 1: Producción de leche
def produccion_leche(V, K, X):


    leche_por_dia = V * X
    leche_por_semana = leche_por_dia * 7
    return leche_por_semana
# problema 2: Produccion de huevos
def produccion_huevos(A):
 
    gallinas_rapidas = A // 2 
    gallinas_lentas = A - gallinas_rapidas  

    huevos_rapidas_mes = gallinas_rapidas * (30 // 3)
    huevos_lentas_mes = gallinas_lentas * (30 // 5)

    huevos_totales = huevos_rapidas_mes + huevos_lentas_mes
    return huevos_totales

leche_semanal = produccion_leche(V, K, X)
huevos_mensuales = produccion_huevos(A)

print("Producción de leche por semana:", leche_semanal, "litros")
print("Producción de huevos en un mes:", huevos_mensuales, "huevos")
