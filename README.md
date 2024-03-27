# Anotações sobre o aprendizado da liguagem Java

## Fundamentos de Java

### Introdução
Java é uma linguagem de programação de alto nível, orientada a objetos e projetada para ter o menor número de dependências de implementação possível. É uma linguagem de programação geral que é classificada como de propósito geral, concorrente, orientada a objetos e baseada em classes.

### Sintaxe Básica
***Case Sensitivity:*** Java é sensível a maiúsculas e minúsculas, o que significa que identificadores como Hello e hello teriam significados diferentes em Java.

***Nomes de Classes:*** Por convenção, os nomes de classes em Java começam com uma letra maiúscula.

***Nomes de Métodos:*** Todos os nomes de métodos devem começar com uma letra minúscula. Se o nome contiver várias palavras, cada palavra interna deve começar com uma letra maiúscula.

***Nome do Arquivo:*** O nome do arquivo de programa Java deve corresponder exatamente ao nome da classe e terminar com a extensão .java.

## Estrutura de um Programa Java
Um programa Java típico pode ser estruturado da seguinte forma:

```java

public class Main {
    public static void main(String[] args) {
        // Código do programa aqui
    }
}

```

***Classe:*** Tudo em Java está associado a classes e objetos, com a exceção de variáveis primitivas.

***Métodos:*** Cada aplicativo Java tem um método main que serve como o ponto de entrada para o programa.

## Tipos de Dados
Java suporta vários tipos de dados, classificados em dois grupos:

***Tipos Primitivos:*** Incluem byte, short, int, long, float, double, boolean, e char.

***Tipos Não Primitivos:*** Incluem Classes, Interfaces, e Arrays.

## Variáveis
Em Java, as variáveis devem ser declaradas antes de serem usadas. A sintaxe básica é:

```java

//tipo nomeVariavel = valor;

```

## Operadores
Java fornece um rico conjunto de operadores para manipular variáveis. Eles podem ser classificados como:

***Operadores Aritméticos:*** **+, -, *, /, %**
***Operadores de Comparação:*** **==, !=, >, <, >=, <=**
***Operadores Lógicos:*** **&&, ||, !**

## Controle de Fluxo
Java suporta as estruturas de controle de fluxo padrões:

***Decisões:*** **if, if...else, switch**
***Loops:*** **for, while, do...while**

# Arrays
Arrays em Java são usados para armazenar múltiplos valores em uma única variável. Eles são declarados como:

```java
tipo[] nomeArray = new tipo[tamanho];
```

## Orientação a Objetos
Os principais conceitos da programação orientada a objetos em Java são:

***Classe e Objeto***
***Herança***
***Polimorfismo***
***Encapsulamento***
***Abstração***

## Conclusão
Java é uma linguagem poderosa e flexível com muitos mais conceitos e características para explorar. Este guia cobriu apenas os fundamentos para começar.
