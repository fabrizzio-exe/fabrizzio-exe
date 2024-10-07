# Programa para ingresar las ventas de un vendedor

ventas = []  # Lista para almacenar las ventas

while True:
    venta = float(input("Ingrese el monto de la venta (ingrese 0 para terminar): "))
    if venta == 0:
        break  # Termina el ingreso de ventas
    ventas.append(venta)

# Si se ingresaron ventas, mostrar los resultados
if ventas:
    venta_total = sum(ventas)
    venta_maxima = max(ventas)
    venta_minima = min(ventas)

    print(f"\nVenta total: {venta_total}")
    print(f"Venta más alta: {venta_maxima}")
    print(f"Venta más baja: {venta_minima}")
else:
    print("No se ingresaron ventas.")
