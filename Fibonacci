fun main() {
    print("Digite quantos termos da sequência de Fibonacci você deseja: ")
    val n = readLine()?.toIntOrNull() ?: return

    var atual = 1 // Armazena a soma de dois termos consecutivos: anterior + atual

    for (i in 1..n) {
        val anterior = atual - (if (i > 2) anteriorFibo(i - 1) else 0)
        println(anterior)
        atual += anterior
    }
}

fun anteriorFibo(n: Int): Int {
    var atual = 1
    var anterior = 0

    repeat(n - 1) {
        val temp = atual
        atual += anterior
        anterior = temp
    }

    return anterior
}
