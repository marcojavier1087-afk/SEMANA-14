ALUMNO MARCOS JAVIER PAREDES GUAMAN

PRIMER SEMESTRE 


def calcular_precio_total(precio_por_persona, cantidad_personas, descuento):
    """
    Calcula el precio total de un paquete turístico.
    Parámetros:
        precio_por_persona (float): costo del tour por persona
        cantidad_personas (int): número de turistas
        descuento (float): porcentaje de descuento (ej. 0.10 = 10%)
    Retorna:
        float: precio total a pagar
    """
    subtotal = precio_por_persona * cantidad_personas
    total = subtotal - (subtotal * descuento)
    return total


precio_tour = 25.0
turistas = 4
descuento_grupo = 0.10

total_a_pagar = calcular_precio_total(precio_tour, turistas, descuento_grupo)

print(f"El precio total del tour para {turistas} personas es: ${total_a_pagar:.2f}")
