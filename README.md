# Sistema-de-calificaciones-con-arreglos-y-vectores-
El programa permite visualizar, modificar y analizar los datos almacenados en un arreglo

## Objetivo del programa
Aplicar los conceptos de arreglos, índices, ciclos y condiciones para desarrollar un programa funcional que procese información almacenada en un vector.

## Lenguaje utilizado
Python 3.x

## Funcionalidades desarrolladas
- Mostrar todas las calificaciones almacenadas.
- Acceder a una calificación mediante su índice.
- Calcular el promedio general.
- Identificar la calificación más alta y más baja.
- Contar cuántos estudiantes aprobaron y reprobaron.
- Modificar una calificación dentro del arreglo.
- Mostrar el vector actualizado después de la modificación.

## Instrucciones para ejecutar el programa
1. Clonar el repositorio desde GitHub.
2. Abrir una terminal en la carpeta del proyecto.
3. Ejecutar el archivo principal con: Python 3

#Código
# Vector inicial de calificaciones
calificaciones = [85, 67, 92, 74, 58]

print("--- SISTEMA DE CALIFICACIONES BÁSICO ---")
print("Vector original:", calificaciones)
print("-" * 45)

# 1. Mostrar todas las calificaciones
print("1. Todas las calificaciones:")
print(calificaciones)

# 2. Mostrar una calificación utilizando su índice (ejemplo: índice 2)
indice = 2
print(f"\n2. La calificación en el índice {indice} es: {calificaciones[indice]}")

# 3. Calcular el promedio
promedio = sum(calificaciones) / len(calificaciones)
print(f"\n3. El promedio de las calificaciones es: {promedio}")

# 4. Identificar la calificación más alta
mas_alta = max(calificaciones)
print(f"\n4. La calificación más alta es: {mas_alta}")

# 5. Identificar la calificación más baja
mas_baja = min(calificaciones)
print(f"\n5. La calificación más baja es: {mas_baja}")

# 6. Contar cuántos estudiantes aprobaron (nota >= 70)
aprobados = 0
for nota in calificaciones:
    if nota >= 70:
        aprobados += 1
print(f"\n6. Cantidad de estudiantes aprobados: {aprobados}")

# 7. Contar cuántos estudiantes reprobaron (nota < 70)
reprobados = 0
for nota in calificaciones:
    if nota < 70:
        reprobados += 1
print(f"\n7. Cantidad de estudiantes reprobados: {reprobados}")

# 8. Modificar una calificación (por ejemplo, cambiar la del índice 1 a 90)
print("\n8. Modificando la calificación del índice 1 (que era 67) por 90...")
calificaciones[1] = 90

# 9. Mostrar nuevamente el vector actualizado
print("\n9. Vector actualizado:")
print(calificaciones)
