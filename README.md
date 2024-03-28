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


## Comentários 

Comentários em Java são anotações no código-fonte que são ignoradas pelo compilador. Eles são usados para explicar o código, tornando-o mais compreensível para humanos. Isso pode incluir notas sobre a funcionalidade de um segmento de código, esclarecimentos sobre a lógica complexa, ou instruções sobre como o código deve ser usado ou modificado no futuro. Em Java, existem três principais tipos de comentários:

1. **Comentários de linha única**: Começam com `//`. Tudo à direita das duas barras, na mesma linha, é tratado como um comentário e é ignorado pelo compilador.
 
```java
 // Isso é um comentário de linha única em Java.
 int i = 10; // Isso também é um comentário, seguindo uma instrução.
 ```

2. **Comentários de múltiplas linhas (ou comentários em bloco)**: Começam com `/*` e terminam com `*/`. Tudo entre `/*` e `*/`, independente de quantas linhas ocupe, é tratado como um comentário. Eles são úteis para comentários mais extensos ou para temporariamente desativar partes do código.
 
```java
 /* Isso é um comentário
 de múltiplas linhas.
 Ele pode abranger várias linhas. */
 ```

3. **Comentários de documentação (JavaDoc)**: Começam com `/**` e terminam com `*/`. Eles são usados para gerar documentação HTML a partir do código-fonte. Comentários JavaDoc podem incluir tags que fornecem informações adicionais para a documentação, como parâmetros de métodos, valores de retorno, exceções lançadas e mais.
 
```java
 /**
 * Esta é uma função JavaDoc que soma dois números.
 *
 * @param a Primeiro número a ser somado.
 * @param b Segundo número a ser somado.
 * @return A soma de a e b.
 */
 public int soma(int a, int b) {
 return a + b;
 }
 ```

Usar comentários de maneira eficaz é uma habilidade importante no desenvolvimento de software. Eles devem ser claros, concisos e relevantes, ajudando outros desenvolvedores a entender o propósito e o funcionamento do código sem introduzir ruído ou informações desatualizadas. É uma prática recomendada revisar e atualizar os comentários conforme o código evolui.


## Váriaveis e Cosntantes

Em Java, tanto variáveis quanto constantes são fundamentais para armazenar dados que seu programa pode manipular. Porém, elas têm propósitos e regras de uso distintos. Vamos explorar esses conceitos:

## Variáveis
Variáveis em Java são espaços de memória alocados para armazenar dados que podem ser modificados durante a execução do programa. Cada variável em Java tem um tipo de dado específico, que determina o tamanho e o layout da memória da variável, além do intervalo de valores que ela pode armazenar, e o conjunto de operações que podem ser aplicadas a ela.

## Declaração de Variáveis
Para declarar uma variável em Java, você deve especificar o tipo de dado, seguido pelo nome da variável. Opcionalmente, você pode inicializá-la com um valor. Por exemplo:

```java
int idade = 30;
double salario = 4550.50;
String nome = "Carlos";
```

Neste exemplo, idade é uma variável do tipo int que armazena números inteiros, salario é uma variável do tipo double que armazena números de ponto flutuante (com casas decimais), e nome é uma variável do tipo String que armazena uma sequência de caracteres (texto).

## Constantes
Constantes são espaços de memória para armazenar dados que não podem ser modificados uma vez que um valor inicial é atribuído. Em Java, constantes são definidas com a palavra-chave final.

## Declaração de Constantes
Para declarar uma constante em Java, use a palavra-chave final, seguida pelo tipo de dado, nome da constante e, obrigatoriamente, um valor inicial. Uma vez atribuído um valor a uma constante, este não pode ser alterado. Por exemplo:

```java
final int NUMERO_DE_DIAS_SEMANA = 7;
final double PI = 3.14159;
```

Neste exemplo, NUMERO_DE_DIAS_SEMANA e PI são constantes que armazenam, respectivamente, o número de dias em uma semana e a aproximação do valor de PI. Tentar alterar o valor de uma constante após sua inicialização resultará em um erro de compilação.

## Práticas Recomendadas

***Variáveis:*** Use nomes significativos para variáveis, escolhendo nomes que reflitam o propósito da variável no programa. Isso aumenta a legibilidade do código.

***Constantes:*** Use constantes para representar valores fixos que não mudam ao longo do tempo, como configurações estáticas, valores de configuração ou qualquer outro tipo de valor que deve permanecer constante ao longo da execução do programa.

O uso adequado de variáveis e constantes ajuda a criar um código mais seguro, pois previne modificações não intencionais em partes do programa que deveriam permanecer estáticas, e também torna o código mais legível e fácil de manter.



## Inferências de Tipos


A inferência de tipos é um recurso que permite ao compilador automaticamente determinar o tipo de uma variável, baseado no valor com que ela é inicializada. Em Java, a inferência de tipos foi introduzida na versão 10, através da palavra-chave var. Esse recurso é particularmente útil para melhorar a legibilidade do código em situações onde o tipo exato da variável é evidente a partir do contexto.

## Como Funciona
Quando você usa var para declarar uma variável, não é necessário especificar explicitamente seu tipo; o compilador irá inferir o tipo com base no valor atribuído à variável no momento da sua inicialização. É importante notar que o uso de var só é permitido quando a variável é inicializada na declaração, pois o compilador precisa do valor de inicialização para determinar o tipo da variável.

Exemplo de Uso

```java

var numero = 10; // Inferido como int
var mensagem = "Olá, mundo!"; // Inferido como String
var lista = new ArrayList<String>(); // Inferido como ArrayList<String>

```

Nesses exemplos, o compilador infere o tipo de numero como int, o tipo de mensagem como String, e o tipo de lista como ArrayList<String>, baseado nos valores com que elas são inicializadas.

## Vantagens
Legibilidade do Código: O código se torna mais limpo e mais fácil de ler, especialmente em casos onde o tipo é longo ou complicado.

***Menos Verbosidade:*** Reduz a necessidade de especificar explicitamente tipos complexos, tornando o código mais conciso.

## Limitações e Considerações
***Inicialização Obrigatória:*** Variáveis declaradas com var devem ser inicializadas na sua declaração. Isso é necessário para que o compilador possa inferir o tipo.

***Uso Local:*** A inferência de tipos com var só é permitida em contextos locais, como dentro de métodos. Não é possível usar var para declarar campos de classe, parâmetros de métodos ou tipos de retorno.

***Clareza:*** Embora var possa tornar o código menos verboso, seu uso excessivo ou inadequado pode tornar o código menos claro, especialmente em situações onde o tipo não é evidente. É importante encontrar um equilíbrio para manter o código compreensível.

A introdução da inferência de tipos com var em Java segue uma tendência de muitas outras linguagens de programação que suportam essa funcionalidade, ajudando a tornar o código mais conciso sem sacrificar a segurança de tipo que é central para a linguagem Java.

## Tipos Primitivos

Em Java, os tipos primitivos são os blocos de construção mais básicos da linguagem, representando valores simples que não compartilham estado com outros valores. Existem oito tipos primitivos em Java, cada um com um tamanho específico e um valor padrão. Vamos explorá-los:

**1. byte***
***Descrição:*** Tipo inteiro de 8 bits com sinal.
***Faixa de Valores:*** De -128 a 127.
***Uso Comum:*** Útil para economizar memória em matrizes grandes, principalmente em lugar de int.

**2. short***
***Descrição:*** Tipo inteiro de 16 bits com sinal.
***Faixa de Valores:*** De -32.768 a 32.767.
***Uso Comum:*** Também pode ser usado para economizar memória como o byte.

**3. int***
***Descrição:*** Tipo inteiro de 32 bits com sinal.
***Faixa de Valores:*** De -2^31 a 2^31-1.
***Uso Comum:*** Geralmente o tipo padrão usado para números inteiros, a menos que haja uma preocupação específica de memória.

**4. long***
***Descrição:*** Tipo inteiro de 64 bits com sinal.
***Faixa de Valores:*** De -2^63 a 2^63-1.
***Uso Comum:*** Quando você precisa de um intervalo de valores maior do que o fornecido por int.

**5. float***
***Descrição:*** Tipo ponto flutuante de precisão simples de 32 bits.
***Faixa de Valores:*** Cobrem uma enorme faixa de valores; aproximadamente ±3.40282347E+38F (6-7 dígitos significativos decimais).
***Uso Comum:*** Usado para economizar memória em matrizes grandes de números de ponto flutuante; menos precisão do que double.

**6. double***
***Descrição:*** Tipo ponto flutuante de precisão dupla de 64 bits.
***Faixa de Valores:*** Cobrem uma enorme faixa de valores; aproximadamente ±1.79769313486231570E+308 (15 dígitos significativos decimais).
***Uso Comum:*** O tipo padrão para números de ponto flutuante.

**7. boolean**
***Descrição:*** Tipo lógico que pode ter apenas dois valores: true (verdadeiro) ou false (falso).
***Uso Comum:*** Controles de fluxo condicionais, loops e variáveis de flag.

**8. char**
***Descrição:*** Tipo caractere de 16 bits representando um caractere Unicode.
***Faixa de Valores:*** De '\u0000' (ou 0) a '\uffff' (ou 65.535 inclusive).
***Uso Comum:*** Armazenar caracteres individuais.

## Características dos Tipos Primitivos
***Não são objetos:*** Diferente de outros tipos em Java, os tipos primitivos não são objetos. Isso significa que eles não têm métodos ou propriedades.

***Tamanho fixo:*** Cada tipo primitivo tem um tamanho de memória fixo, o que os torna muito eficientes.

***Valor padrão:*** Se um tipo primitivo for declarado como uma variável de classe ou de instância e não for inicializado, ele terá um valor padrão (como 0 para tipos numéricos, false para boolean e '\u0000' para char).

Os tipos primitivos são fundamentais na programação Java e são usados extensivamente para a manipulação de dados básicos e controle de fluxo em programas.


## Notação Ponto


A notação de ponto em Java é uma maneira de acessar membros (variáveis ou métodos) de uma classe ou de um objeto. Essa notação é fundamental na programação orientada a objetos, pois permite a interação com os atributos e métodos das classes de uma maneira clara e organizada. A sintaxe básica utiliza um ponto (.) para separar o objeto ou classe do membro que se deseja acessar. Aqui estão alguns exemplos de como ela é utilizada:

### Acessando Membros Estáticos
Quando se quer acessar membros estáticos de uma classe (aqueles que pertencem à classe em si, e não a uma instância específica dela), usa-se o nome da classe seguido de um ponto e o nome do membro estático. Por exemplo:

```java
Math.PI // Acessa a constante PI da classe Math.
Math.sqrt(25) // Chama o método estático sqrt (raiz quadrada) da classe Math.
```

### Acessando Membros de Objetos
Para acessar campos (atributos) ou métodos de um objeto, você usa o nome do objeto seguido de um ponto e o nome do campo ou método. Por exemplo:

```java
String texto = "Olá, mundo!";
int tamanho = texto.length(); // Chama o método length de um objeto da classe String.
System.out.println(texto); // Acessa o método estático println da classe System para imprimir o texto.
```

### Encadeamento de Métodos
A notação de ponto também permite o encadeamento de chamadas de métodos, quando um método retorna um objeto, permitindo assim a chamada de outro método sem necessidade de armazenar o objeto intermediário em uma variável. Por exemplo:

```java
String resultado = "Olá, Mundo!".toLowerCase().replace("mundo", "Java");

```

Nesse exemplo, o método toLowerCase() é chamado no objeto string "Olá, Mundo!". O resultado desse método (outra string) é então usado imediatamente para chamar o método replace(), sem a necessidade de armazenar o resultado intermediário em uma variável separada.

### Acessando Atributos de Objetos
A notação de ponto também é usada para acessar diretamente atributos (campos) de um objeto, desde que esses atributos sejam acessíveis de acordo com as regras de visibilidade (public, protected, default, private) da linguagem Java.

```java
Carro meuCarro = new Carro();
meuCarro.cor = "Azul"; // Acessa e modifica o atributo 'cor' do objeto 'meuCarro'.
System.out.println(meuCarro.cor); // Imprime o valor do atributo 'cor'.

```

Essa notação é essencial para a manipulação de objetos e classes em Java, permitindo uma sintaxe clara e eficiente para a programação orientada a objetos.

## IMPORT

O import em Java é uma declaração que permite ao programador acessar classes ou interfaces de outros pacotes, facilitando o uso de bibliotecas e a organização do código em pacotes separados. Sem o uso de import, seria necessário referenciar cada classe ou interface pelo seu nome completamente qualificado (fully qualified name), incluindo o nome do pacote, o que tornaria o código mais verboso e difícil de manter.

### Como Usar
Para usar uma classe ou interface de outro pacote em seu código, você coloca uma declaração import no início do seu arquivo de código-fonte (após o pacote, caso exista, e antes da declaração da classe ou interface). Há duas maneiras principais de usar import:

- Importação específica: Importa uma única classe ou interface de um pacote. Isso é feito especificando o nome completo da classe ou interface que você deseja importar. Por exemplo:

```java

import java.util.ArrayList;
```

Esse comando importa apenas a classe ArrayList do pacote java.util, tornando-a disponível sem a necessidade de usar seu nome completamente qualificado.

- Importação de pacote (wildcard): Importa todas as classes e interfaces de um pacote específico. Isso é feito utilizando o caractere asterisco (*) após o nome do pacote. Por exemplo:

```java
import java.util.*;
```

Esse comando importa todas as classes e interfaces contidas no pacote java.util, permitindo que você use qualquer uma delas diretamente pelo nome da classe ou interface.

### Importação Estática
Java também suporta importações estáticas, que permitem acessar membros estáticos (campos e métodos) de uma classe diretamente sem precisar qualificar com o nome da classe. Por exemplo:

```java
import static java.lang.Math.PI;
import static java.lang.Math.sqrt;

public class Teste {
    public static void main(String[] args) {
        double area = PI * sqrt(25);
    }
}
```

Neste exemplo, PI e sqrt são acessados diretamente sem a necessidade de prefixá-los com Math., graças à importação estática.

### Benefícios do Uso de import

- Legibilidade: O código se torna mais legível, pois evita a repetição do nome do pacote toda vez que uma classe ou interface for usada.
- Manutenção: Facilita a manutenção do código, já que mudanças no pacote de uma classe usada só precisam ser ajustadas na declaração de import.
- Organização: Promove uma melhor organização do código, permitindo que os desenvolvedores agrupem funcionalidades relacionadas em pacotes distintos.

### Considerações
Importar com o wildcard (*) é conveniente, mas pode levar a conflitos de nomes se dois pacotes contiverem classes ou interfaces com o mesmo nome.
Java importa automaticamente todas as classes no pacote java.lang, então não é necessário usar import para classes como String, Math, entre outras desse pacote.