# Recursividad

fun main() {
    val resultado = multiplicar(1, 5)
    println("El producto de los números del 1 al 5 es: $resultado")
}

fun multiplicar(actual: Int, limite: Int): Int {
    return if (actual > limite) {
        1 // Caso base: el producto de no multiplicar nada es 1
    } else {
        actual * multiplicar(actual + 1, limite) // Llamada recursiva
    }
}
