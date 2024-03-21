<div class="header">
    <img align="center" src="https://seeklogo.com/images/C/c-sharp-c-logo-02F17714BA-seeklogo.com.png" width="100"/> The Script.

# _Tipos de Dados_

</div>

- [Tipos](Tipos)

<br>

# Tipos

Em C#, os tipos de dados são categorizados em tipos de valor e tipos de referência. Aqui estão alguns dos principais tipos de dados em C#.

O C# é uma linguagem fortemente tipada, o que significa que os tipos são extremamente relevantes para uma programação de maior qualidade.

## Tipo de valor

| Tipo      | Descrição                                     | Faixa de Valores                                       |
| --------- | --------------------------------------------- | ------------------------------------------------------ |
| `sbyte`   | 8 bits com sinal                              | -128 a 127                                             |
| `byte`    | 8 bits sem sinal                              | 0 a 255                                                |
| `short`   | 16 bits com sinal                             | -32,768 a 32,767                                       |
| `ushort`  | 16 bits sem sinal                             | 0 a 65,535                                             |
| `int`     | 32 bits com sinal                             | -2,147,483,648 a 2,147,483,647                         |
| `uint`    | 32 bits sem sinal                             | 0 a 4,294,967,295                                      |
| `long`    | 64 bits com sinal                             | -9,223,372,036,854,775,808 a 9,223,372,036,854,775,807 |
| `ulong`   | 64 bits sem sinal                             | 0 a 18,446,744,073,709,551,615                         |
| `float`   | Ponto flutuante de precisão simples           | Aprox. 6-9 dígitos de precisão                         |
| `double`  | Ponto flutuante de precisão dupla             | Aprox. 15-17 dígitos de precisão                       |
| `decimal` | Tipo de ponto fixo com alta precisão          | 28-29 dígitos de precisão                              |
| `char`    | Representa um caractere Unicode de 16 bits    | '\u0000' a '\uffff'                                    |
| `bool`    | Representa um valor booleano verdadeiro/falso | True ou False                                          |
| `enum`    | Define um conjunto de constantes nomeadas     | Valores definidos pelo usuário                         |

## Tipo de referência

| Tipo        | Descrição                                                                      |
| ----------- | ------------------------------------------------------------------------------ |
| `class`     | Define uma referência a um objeto                                              |
| `string`    | Representa uma sequência de caracteres Unicode                                 |
| `object`    | Representa qualquer tipo de objeto                                             |
| `interface` | Define um contrato que as classes podem implementar                            |
| `arrays`    | Coleção de elementos do mesmo tipo, acessíveis por um índice                   |
| `delegate`  | Representa um tipo que pode encapsular um método com uma assinatura específica |

## Classes e Objetos

Classes são os Tipos mais fundamentais do C#. Classes permitem a criação de instâncias, instâncias essas conhecidas como objetos. As classes podem possuir comportamentos próprios, como _polymorphism_, que é um mecanismo em que classes podem ser extendidas baseadas numa outra.

A classe precisa especificar:

- Atributos e modificações da classe
- O nome da classe
- A classe base (quando herdando de uma classe base)
- As interfaces implementadas pela classe
- O cabeçalho é seguiodo elo corpo da classe, que consiste em uma lista de declarações de membros escritas entre os delimitadores `{ e }`

O código as seguir mostra uma declaração de uma classe simples chamada `Point`:

```C#
public class Point
{
    public int X { get; }
    public int Y { get; }

    public Point(int x, int y) => (X, Y) = (x, y);
}
```

Instâncias dessa classe podem ser criadas utilizando o operador `new`. O código a seguir cria dois objetos `Point` e armazena referências desses objetos em duas variávei:

```C#
var p1 = new Point(0, 0);
var p2 = new Point(10, 20);
```

<div align="center">

# AUTOR

</div>

<div class="footer">
    <table align="center">
        <tr>
            <td align="center"> 
		        <a href="https://github.com/yagopeixinho">
			        <img src="https://avatars.githubusercontent.com/u/81770553?v=4" width="100px;" alt="Imagem de Yago Peixinho">    
            <br>
		            <sub>
		                <b>Yago Peixinho </b>
		            </sub>
		        </a> 
	        </td> 
        </tr>
   </table>
</div>
<div>

###### Referências desse documento

- https://learn.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types

</div>
