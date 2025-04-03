ANCHO_TERRENO = int(input("Ingrese ancho del terreno:"))
LARGO_TERRENO = int(input("Ingrese largo del terreno:"))
LADO_SEMBRADIO = int(input("Ingrese el lado de cada sembradio:"))
if LADO_SEMBRADIO > ANCHO_TERRENO or LADO_SEMBRADIO > LARGO_TERRENO:
    print("Error: No hay solucion posible")
elif LADO_SEMBRADIO <= ANCHO_TERRENO and LADO_SEMBRADIO <= LARGO_TERRENO:
    AREA_TERRENO = (ANCHO_TERRENO * LARGO_TERRENO)
    AREA_SEMBRADIO = (LADO_SEMBRADIO * LADO_SEMBRADIO)
    FILAS = ANCHO_TERRENO // LADO_SEMBRADIO
    COLUMNAS = LARGO_TERRENO // LADO_SEMBRADIO
    n = FILAS * COLUMNAS
    TOTAL_SEMBRADO = AREA_SEMBRADIO * n
    print("Se plantaran", n,"sembradios de", LADO_SEMBRADIO,"x", LADO_SEMBRADIO,"m")
    print("El total sembrado sera de", TOTAL_SEMBRADO,"m2")
    SOBRANTE = AREA_TERRENO - TOTAL_SEMBRADO
    print("El sobrante no sembrado en el terreno será de", SOBRANTE,"m2")
    if n <= 200:
        HUMEDAD = 350
        TEMPERATURA = 450
        PH = 1400
    elif 200<n<=400:
        HUMEDAD = 300
        TEMPERATURA = 350
        PH = 1200
    elif 400 < n <= 1000:
        HUMEDAD = 250
        TEMPERATURA = 250
        PH = 1000
    elif n > 1000:
        HUMEDAD= 200
        TEMPERATURA= 150
        PH= 800
    COSTO_SENSORES = ((HUMEDAD*4)*TOTAL_SEMBRADO)+(TEMPERATURA*TOTAL_SEMBRADO)+((PH*3)*TOTAL_SEMBRADO)
    VALOR_SENSORES = COSTO_SENSORES/1000000
    VALOR_TRUNCADO = round(VALOR_SENSORES, 2)
    print("El costo de los sensores será: M$",VALOR_TRUNCADO)
    SUBSIDIO = TOTAL_SEMBRADO//10000
    DESCUENTO = round(SUBSIDIO, 0)
    VALOR = 15*DESCUENTO
    print("El subsidio del gobierno será: M$", VALOR)
    MONTO_FINAL= round(VALOR_TRUNCADO-VALOR, 2)
    print("Costo total de la plantación: M$",MONTO_FINAL)