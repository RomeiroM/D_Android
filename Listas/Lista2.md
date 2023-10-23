## Lista de Estruturas de Repetições
#### 1️⃣ Escreva um programa que imprima os números de 1 a 10 utilizando um loop while.

````kotlin
fun main(){
    var num : Int = 1  // 1
    while(num <= 10){ // 2
        println(num) // 3
        num++       // 4
    }
}
````

<details>
<summary>Explicação das linhas de código</summary>

- 1️⃣ Inicializando uma variável mutável (var) do tipo inteiro (Int) e atribuindo a ela o valor 1
- 2️⃣ Laço de repetição while com a seguinte condição: Enquanto (while) a variável “num” for menor ou igual (<=) a 10 execute o código.
- 3️⃣ Essa linha vai exibir o número que estiver na variável “num”.
- 4️⃣ "num++" significa um [auto incremento](https://www.galirows.com.br/meublog/programacao/diferenca-entre-operador-incremento-antes-depois/) onde a variável “num” vai receber o valor dela mesma e soma mais 1.
  - Ex: Se _"soma = 4"_ ; Então _"soma++"_ será igual a 5 porque 4 + 1 = 5.

</details>

#### 2️⃣ Escreva um programa que imprima os números pares de 2 a 20 utilizando um loop for.
````kotlin
fun main(){
    for(num in 2..20 step 2){ // 1
        println(num)        // 2
    }
}
````

<details>
<summary>Explicação das linhas de código</summary>

- 1️⃣ A estrutura de repetição “for” pode ser lida como: Para “num” começado em 2 até 20 (2..20) pule dois números (step 2).
- 2️⃣ Esta linha vai exibir o número que estiver na variável “num” que a cada repetição vai ganhar um valor diferente.

</details>

#### 3️⃣ Escreva um programa que imprima os números ímpares de 1 a 15 utilizando um loop do-while.
````kotlin
fun main(){
    var num = 1  // 1
    do{         // 2
        println(num)// 3
        num +=2     // 4  
       } while (num < 15)// 5
}
````

<details>
<summary>Explicação das linhas de código</summary>

- 1️⃣ Inicialização de uma [variável mutável](https://acervolima.com/variaveis-kotlin/) (var) do tipo inteiro, atribuindo o valor 1 a ela.
- 2️⃣ O loop “do…while” executará o bloco de código uma vez, antes de verificar se a condição é verdadeira, então repetirá o loop enquanto a condição for verdadeira.
- 3️⃣ Esta linha vai exibir o número que estiver na variável “num” que a cada repetição vai ganhar um valor diferente.
- 4️⃣ _“num+=2”_ significa que o programa esta somando duas unidades a cada loop.
  - Ex: Se _"num = 5"_; Então _“num+=2”_ será igual a 7 porque 5 + 2 = 7.
- 5️⃣ Nesta linha o programa vai testar a condição de parada: Enquanto a variável _“num”_ for menor do que 15 execute novamente o loop.

</details>

#### 4️⃣ Escreva um programa que imprima a soma dos números de 1 a 100 utilizando um loop for.

````kotlin
fun main(){
    var soma = 0         // 1
    for(num in 1..100){ // 2
        soma+= num     // 3
    } 
    println(soma)     //4
}
````

<details>
<summary>Explicação das linhas de código</summary>

- 1️⃣ Inicialização de uma [variável mutável](https://acervolima.com/variaveis-kotlin/) (var) do tipo inteiro, atribuindo o valor 0 a ela.
- 2️⃣ A estrutura de repetição _“for”_ pode ser lida como: Para _“num”_ começado em 1 até 100 (_1..100_) execute o código abaixo.
- 3️⃣ _"soma+="_ é um [auto incremento](https://www.galirows.com.br/meublog/programacao/diferenca-entre-operador-incremento-antes-depois/) onde a variável “soma” vai receber o valor de _"num"_ e soma a ela mesma.
  - Ex: Se _"soma = 4"_ e _"num = 2"_; Então _"soma+= num"_ será igual a 6 porque 4 + 2 = 6.
- 4️⃣ Esta linha vai exibir a soma dos números de 1 a 100.

</details>

#### 5️⃣ Escreva um programa que leia um número inteiro do usuário e imprima a tabuada desse número utilizando um loop for.

````kotlin
fun main(){
    println("Tabuada do número:")         // 1
    var numTabuada = readLine()!!.toInt()// 2
    for(num in 1..10){                  // 3
        println("$numTabuada X $num = "+ num*numTabuada) // 4
    }
}
````

<details>
<summary>Explicação das linhas de código</summary>

- 1️⃣ Mensagem para o usuário.
- 2️⃣ Inicialização de uma [variável mutável](https://acervolima.com/variaveis-kotlin/) (var) que vai receber um valor inteiro inserido pelo usuário(_readLine()!!.toInt()_) sem checagem de valores nulos (_!!_).
- 3️⃣ A estrutura de repetição _“for”_ pode ser lida como: Para _“num”_ começado em 1 até 10 (_1..10_) execute o código abaixo.
- 4️⃣ Esta linha vai mostrar ao usuário a tabuada do número escolhido.
  - Exemplo de saída: _7 X 4 = 28_ 

</details>

#### 6️⃣ Escreva um programa que leia um número inteiro do usuário e imprima os seus divisores utilizando um loop while.

````kotlin
fun main(){
    println("Digite um número:")       // 1
    var numDiv = readLine()!!.toInt() // 2
    var cont = 1                     // 3
    while(cont <= numDiv){          // 4
        if((numDiv % cont) == 0){  // 5
            println(cont)         // 6
        }
        cont++                  // 7
    }
}
````

<details>
<summary>Explicação das linhas de código</summary>

- 1️⃣ Mensagem para o usuário.
- 2️⃣ Inicialização de uma [variável mutável](https://acervolima.com/variaveis-kotlin/) (var) que vai receber um valor inteiro inserido pelo usuário(_readLine()!!.toInt()_) sem checagem de valores nulos (_!!_).
- 3️⃣ Inicializando uma variável mutável (_var_) do tipo inteiro e atribuindo a ela o valor 1.
- 4️⃣ Laço de repetição while com a seguinte condição: Enquanto (while) a variável _“cont”_ for menor ou igual (<=) a variável _"numDiv"_ execute o código.
- 5️⃣ Esta condicional _“if”_ pode ser lida como: Se (_if_) o [resto da divisão](https://brasilescola.uol.com.br/matematica/o-resto-divisao.htm) (_%_) por _“cont”_ for igual a zero (_== 0_) execute o código.
- 6️⃣ Esta linha vai exibir os divisores do número escolhido.
- 7️⃣ "cont++" é um [auto incremento](https://www.galirows.com.br/meublog/programacao/diferenca-entre-operador-incremento-antes-depois/) onde a variável “cont” vai receber o valor dela mesma e soma mais 1.
  - Ex: Se _"cont = 4"_ ; Então _"cont++"_ será igual a 5 porque 4 + 1 = 5.

</details>

#### 7️⃣ Escreva um programa que leia vários números inteiros do usuário até que o número 0 seja digitado. Em seguida, imprima a média dos números lidos utilizando um loop do-while.

````kotlin
fun main() {
    var soma = 0 // 1
    var cont = 0 // 2
    var num: Int // 3
    println("Digite um número diferente de zero:")// 4 
    do{                                         // 5
        num =  readLine()!!.toInt()            // 6
        if(num != 0){                         // 7
            soma+= num                       // 8 
            cont++                          // 9
        } 
    }while(num != 0)                      // 10
    println("Média: "+ soma / cont)      // 11
}

````

<details>
<summary>Explicação das linhas de código</summary>

- 1️⃣ Inicialização de uma [variável mutável](https://acervolima.com/variaveis-kotlin/) (var) do tipo inteiro, atribuindo o valor 0 a ela.
- 2️⃣ Inicialização de uma [variável mutável](https://acervolima.com/variaveis-kotlin/) (var) do tipo inteiro, atribuindo o valor 0 a ela.
- 3️⃣ Inicialização de uma [variável mutável](https://acervolima.com/variaveis-kotlin/) (var) do tipo inteiro (_Int_) sem atribuição de valor.
- 4️⃣ Exibe uma mensagem para o usuário.
- 5️⃣ O loop “do…while” executará o bloco de código uma vez, antes de verificar se a condição é verdadeira, então repetirá o loop enquanto a condição for verdadeira.
- 6️⃣ Inicialização de uma [variável mutável](https://acervolima.com/variaveis-kotlin/) (var) que vai receber um valor inteiro inserido pelo usuário ( _readLine()!!.toInt()_ ) sem checagem de valores nulos ( _!!_ ).
- 7️⃣ Nesta linha o programa vai testar a condição de parada: Enquanto a variável _“num”_ for diferente de zero (_!= 0_) execute novamente o loop.
- 8️⃣  _"soma+= num"_ é um [auto incremento](https://www.galirows.com.br/meublog/programacao/diferenca-entre-operador-incremento-antes-depois/) onde a variável “soma” vai receber o valor de _"num"_ e soma a ela mesma.
  - Ex: Se _"soma = 4"_ e _"num = 2"_; Então _"soma+= num"_ será igual a 6 porque 4 + 2 = 6.
- 9️⃣ "cont++" é um [auto incremento](https://www.galirows.com.br/meublog/programacao/diferenca-entre-operador-incremento-antes-depois/) onde a variável “cont” vai receber o valor dela mesma e soma mais 1.
  - Ex: Se _"cont = 4"_ ; Então _"cont++"_ será igual a 5 porque 4 + 1 = 5.

- 1️⃣0️⃣ Nesta linha o programa vai testar a condição de parada: Enquanto a variável _“num”_ for diferente de zero ( _!= 0_ ) execute novamente o loop.
- 1️⃣1️⃣ Exibe a média dos números inseridos pelo usuário.

</details>

#### 8️⃣ Escreva um programa que leia um número inteiro do usuário e imprima se ele é primo ou não utilizando um loop for.

````kotlin
fun main(){
    var soma = 0                    // 1
    println("Insira um número:")    // 2
    var num =  readLine()!!.toInt() // 3
    for(i in 1..num){               // 4
        if((num % i)== 0){          // 5
            soma++                  // 6
        }
    }
    if(soma == 2){                  // 7
        println("O número é primo") // 8
    }else{                          // 9
        println("Não é primo")      // 10
    }
}
````

<details>
<summary>Explicação das linhas de código</summary>

- 1️⃣ Inicialização de uma [variável mutável](https://acervolima.com/variaveis-kotlin/) (var) do tipo inteiro, atribuindo o valor 0 a ela.
- 2️⃣ Exibe uma mensagem para o usuário.
- 3️⃣ Inicialização de uma [variável mutável](https://acervolima.com/variaveis-kotlin/) (var) que vai receber um valor inteiro inserido pelo usuário ( _readLine()!!.toInt()_ ) sem checagem de valores nulos ( _!!_ ).
- 4️⃣ A estrutura de repetição _“for”_ pode ser lida como: Para _“i”_ começado em 1 até _"num"_ (_1..num_) execute o código abaixo.
- 5️⃣  Esta condicional _“if”_ pode ser lida como: Se (_if_) o [resto da divisão](https://brasilescola.uol.com.br/matematica/o-resto-divisao.htm) (_%_) por _“i”_ for igual a zero (_== 0_) execute o código.
- 6️⃣ "soma++" é um [auto incremento](https://www.galirows.com.br/meublog/programacao/diferenca-entre-operador-incremento-antes-depois/) onde a variável “soma” vai receber o valor dela mesma e soma mais 1.
  - Ex: Se _"soma = 4"_ ; Então _"soma++"_ será igual a 5 porque 4 + 1 = 5.
- 7️⃣ Esta condicional _“if”_ pode ser lida como: Se (_if_) a variável _"soma"_ for igual a dois (_soma == 2_) execute o código.
- 8️⃣ Exibe uma mensagem de número primo.
- 9️⃣ _"else"_ : Se caso a condição _"if"_ for falsa execute o código a seguir.
- 1️⃣0️⃣ Exibe a mensagem que o número não é primo.

</details>

#### 9️⃣Escreva um programa que leia um número inteiro do usuário e imprima a sequência de Fibonacci até esse número utilizando um loop while.

````kotlin
fun main() {
    print("Sequência de Fibonacci: ")   // 1
    var num = readLine()!!.toInt()     // 2
    var contador: Int = 1             // 3
    var numAtual = 1                 // 4
    var numAnterior = 0              // 5
        
    while(num >= contador){         // 6
        println(numAtual)           // 7
        val proximoNum = numAtual + numAnterior // 8
        numAnterior = numAtual      // 9
        numAtual = proximoNum       // 10
        
        contador++                  // 11
    }    
}
````

<details>
<summary>Explicação das linhas de código</summary>

<div align="center">
  <img src="https://static.mundoeducacao.uol.com.br/mundoeducacao/2023/09/numeros-presentes-na-sequencia-de-fibonacci-relacionados-a-espiral-aurea.jpg" width="500">
  <p>A sequência de Fibonacci é uma sequência de números naturais cujos termos são definidos a partir da soma entre seus dois termos antecessores.</p>
</div>

- 1️⃣ Exibe uma mensagem para o usuário.
- 2️⃣ Inicialização de uma [variável mutável](https://acervolima.com/variaveis-kotlin/) (var) que vai receber um valor inteiro inserido pelo usuário ( _readLine()!!.toInt()_ ) sem checagem de valores nulos ( _!!_ ).
- 3️⃣ Inicialização de uma [variável mutável](https://acervolima.com/variaveis-kotlin/) (var) do tipo inteiro, atribuindo o valor 1 a ela.
- 4️⃣ Inicialização de uma [variável mutável](https://acervolima.com/variaveis-kotlin/) (var) do tipo inteiro, atribuindo o valor 1 a ela.
- 5️⃣ Inicialização de uma [variável mutável](https://acervolima.com/variaveis-kotlin/) (var) do tipo inteiro, atribuindo o valor 0 a ela.
- 6️⃣ Laço de repetição while com a seguinte condição: Enquanto (while) a variável _“num”_ for maior ou igual (>=) a variável _"contador"_ execute o código.
- 7️⃣ Exibe uma mensagem com o número atual.
- 8️⃣ Inicialização de uma [variável imutável](https://acervolima.com/variaveis-kotlin/) (_val_) que vai receber o resultado da soma das variáveis _"numeroAtual"_ e _"numeroAnterior"_.
- 9️⃣ A variável _"numAnterior"_ recebe o valor da variável _"numAtual"_
- 1️⃣0️⃣ A variável _"numAtual"_ recebe o valor da variável _"proximoNum"_ .
- 1️⃣1️⃣ _"contador++"_ é um [auto incremento](https://www.galirows.com.br/meublog/programacao/diferenca-entre-operador-incremento-antes-depois/) onde a variável _“contador”_ vai receber o valor dela mesma e soma mais 1.
  - Ex: Se _"contador = 4"_ ; Então _"contador++"_ será igual a 5 porque 4 + 1 = 5.

</details>

#### 1️⃣0️⃣ Escreva um programa que leia vários números inteiros do usuário até que o número -1 seja digitado. Em seguida, imprima o maior número lido utilizando um loop do-while.

````kotlin
fun main() {
    //Maior número
    var maior: Int = 0                                          // 1
    println("Digite qualquer número ou -1 para sair do loop: ") // 2
    do{                                                         // 3
        val numero = readLine()!!.toInt()                       // 4
        if (numero > maior) maior = numero                      // 5    
    }while(numero != -1)                                        // 6 
    println("O maior número digitado foi: $maior")              // 7
}
````

<details>
<summary>Explicação das linhas de código</summary>

- 1️⃣
- 2️⃣
- 3️⃣
- 4️⃣
- 5️⃣ 
- 6️⃣ 
- 7️⃣ 


</details>

#### 1️⃣1️⃣ Escreva um programa que leia vários números inteiros do usuário até que o número 0 seja digitado. Em seguida, imprima a quantidade de números positivos e negativos lidos utilizando um do while.

````kotlin
fun main() {
    //Positivos e Negativos
    println("Digite qualquer número ou 0 para sair do loop: ") // 1
    var positivo = 0                                 // 2
    var negativo = 0                                // 3
    do{                                            // 4
        val numero = readLine()!!.toInt()         // 5
        if(numero > 0){                       // 6
            positivo++                        // 7
        }else if(numero < 0){                 // 8
            negativo++                        // 9
        }     
    }while(numero != 0)                     // 10
    
    println("Positivos: $positivo\nNegativos: $negativo") // 11
}
````
<details>
<summary>Explicação das linhas de código</summary>

- 1️⃣ Exibe uma mensagem para o usuário.
- 2️⃣
- 3️⃣
- 4️⃣
- 5️⃣ 
- 6️⃣ 
- 7️⃣ 
- 8️⃣ 
- 9️⃣ 
- 1️⃣0️⃣
- 1️⃣1️⃣ Exibe uma mensagem para o usuário.

</details>

#### 1️⃣2️⃣ Escreva um programa que leia um número inteiro do usuário e imprima a sua representação binária utilizando um loop while.

````kotlin
fun main() {
    println("Digite um número")       // 1
    var numero = readLine()!!.toInt()// 2
    var saida = ""                  // 3
    while (numero > 0) {           // 4
        val resto = numero % 2    // 5
        saida = "$resto$saida"   // 6
        numero /= 2             // 7
    }
    println("A representação binária do número é: $saida")// 8
}
````

<details>
<summary>Explicação das linhas de código</summary>

<div align="center">
  <img src="https://github.com/RomeiroM/D_Android/assets/85644789/51ce3556-54ed-4a35-b019-b5ab896cf82b" width="500">
</div>

- 1️⃣ Exibe uma mensagem para o usuário.
- 2️⃣ Inicialização de uma [variável mutável](https://acervolima.com/variaveis-kotlin/) (var) que vai receber um valor inteiro inserido pelo usuário ( _readLine()!!.toInt()_ ) sem checagem de valores nulos ( _!!_ ).
- 3️⃣
- 4️⃣
- 5️⃣ 
- 6️⃣ 
- 7️⃣ 
- 8️⃣ Exibe uma mensagem para o usuário.
  
</details>

#### 1️⃣3️⃣ Escreva um programa que leia um número inteiro do usuário e imprima a soma de seus dígitos utilizando um loop do-while.

[video](https://www.youtube.com/watch?v=5i5hmY6j7dM)

````kotlin
fun main() {
    println("Digite um número:")      // 1
    var numero = readLine()!!.toInt() // 2
    var soma = 0                      // 3
    do{                               // 4
        val ultimoNumero = numero % 10// 5
        soma += ultimoNumero         // 6
        numero = numero / 10       // 7
    }while(numero>0)            // 8
    println(soma)             // 9
}
````
<details>
<summary>Explicação das linhas de código</summary>

- 1️⃣ Exibe uma mensagem para o usuário.
- 2️⃣ Inicialização de uma [variável mutável](https://acervolima.com/variaveis-kotlin/) (var) que vai receber um valor inteiro inserido pelo usuário ( _readLine()!!.toInt()_ ) sem checagem de valores nulos ( _!!_ ).
- 3️⃣
- 4️⃣
- 5️⃣ 
- 6️⃣ 
- 7️⃣ 
- 8️⃣ 
- 9️⃣ Exibe o resultado.

</details>

#### 1️⃣4️⃣ Escreva um programa que leia vários números inteiros do usuário até que o número 0 seja digitado. Em seguida, imprima o segundo maior número lido.

````kotlin
fun main() {
    println("Digite um número:")// 1
    var numMax = 0              // 2
    var segundoMax = 0          // 3
    do{                         // 4
        var numero = readLine()!!.toInt()// 5
        if(numero > numMax){            // 6
            segundoMax = numMax        // 7
            numMax = numero           // 8
        }  
    }while(numero != 0)             // 9
    println("O segundo maior número digitado foi o $segundoMax")//10
}
````
<details>
<summary>Explicação das linhas de código</summary>

- 1️⃣ Exibe uma mensagem para o usuário.
- 2️⃣
- 3️⃣
- 4️⃣
- 5️⃣ Inicialização de uma [variável mutável](https://acervolima.com/variaveis-kotlin/) (var) que vai receber um valor inteiro inserido pelo usuário ( _readLine()!!.toInt()_ ) sem checagem de valores nulos ( _!!_ ).
- 6️⃣ 
- 7️⃣ 
- 8️⃣ 
- 9️⃣ 
- 1️⃣0️⃣ Exibe uma mensagem para o usuário.

</details>

#### 1️⃣5️⃣ Escreva um programa que leia um número inteiro do usuário e imprima se ele é um número perfeito ou não utilizando um loop while.

````kotlin
fun main() {
    println("Digite um número:")       // 1
    var numero = readLine()!!.toInt() // 2
    var cont = 1                     // 3
    var soma = 0                    // 4
    while(numero > cont){         // 5
        if((numero % cont) == 0){// 6
            soma+= cont         // 7
        }
        cont++                // 8
    }
    if(numero == soma) println("Sim") else println("Não") // 9
}
````
<details>
<summary>Explicação das linhas de código</summary>

- 1️⃣ Exibe uma mensagem para o usuário.
- 2️⃣ Inicialização de uma [variável mutável](https://acervolima.com/variaveis-kotlin/) (var) que vai receber um valor inteiro inserido pelo usuário ( _readLine()!!.toInt()_ ) sem checagem de valores nulos ( _!!_ ).
- 3️⃣
- 4️⃣
- 5️⃣ 
- 6️⃣ 
- 7️⃣ 
- 8️⃣ 
- 9️⃣ 

</details>


<details>
<summary>Referências</summary>

- 1️⃣ [Fibonacci](https://mundoeducacao.uol.com.br/matematica/sequencia-fibonacci.htm)
- 2️⃣
- 3️⃣

</details>
