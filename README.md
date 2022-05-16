# README Delphi Helpers 🚀🚀🚀🚀

- Criacao de classes 🔥 🔥 
  - > type TNomeClasse = class🔥 🔥 
  - > Atributos: NomeAtributo : Tipo (pode ser string, integer, etc...)🔥 🔥 
  - > Methods: procedure NomeDoMetodo, Lembrando que esse procedure ele é uma funcao void🔥 🔥 
  - >no implementation inicializar os methods : 🔥 🔥 
  
         procedure TNomeClasse.NomeDoMetodo; 
         begin
         end;
  
  - >A unit é um local onde são agrupados as funções e os procedimentos de maneira que possam vir a ser utilizados pelo programa principal. Além dessas três partes, o código poderá ter a chamada initialization e finalization que são opcionais🔥 🔥  
  - >Unit exemplo:🔥 🔥 
                
          unit NomeDaUnit;

          interface
          uses
            NomeDaUnitQueQueiraUtilizar;

          type NomeClasse = (herancaDentroDosParenteses)
            procedure Metodo1;
            procedure Motodo2;
          end;

          implementation

          { NomeClasse }

          procedure TAdministrador.Metodo1;
          begin

          end;

          procedure TAdministrador.Motodo2;
          begin

          end;
          
          // initialization - opcional
          
          // finalization   - opcional

          end.

## Estrutura de uma classe em Delphi
![Estrutura](https://user-images.githubusercontent.com/58851247/168339639-c6dff1e3-e510-456b-843c-5c10e694e94c.png)

## Operadores ( De atribuição, Aritméticos, Lógicos e Relacionais)🚀🚀
### Operadores Aritméticos🔥 🔥 
>( + ) Adição
>( - ) Subtração
>( * ) Multiplicação
>( / ) Divisão de reais
>( Div ) Divisão de inteiros
>( Mod ) Resto da divisão de inteiros

1 - As operações envolvendo apenas números inteiros resultam sempre em um número inteiro. As operações envolvendo número inteiro com número real resulta sempre em um número real.

### Operador de Atribuição🔥 🔥 
A atribuição de valores é feita usando os caracteres  dois pontos e igual (:=).

Exemplos:

>A := 5;
>D := (a-b)/3;
>Nome := 'Maria';

A esquerda deve estar apenas o nome da variável, enquanto que na direita podem estar constantes, variáveis ou expressões que correspondam ao tipo de dados armazenáveis na variável.

### Operadores Lógicos🔥 🔥 
>AND (E Lógico)
>OR (OU Lógico)
>NOT (NÃO Lógico)

2 - Os operadores lógicos ou operadores booleanos são utilizados quando é necessário trabalhar com o relacionamento de duas ou mais condições ao mesmo tempo, dentro de um if ou dentro de uma estrutura de teste de um loop.

### Operadores Relacionais🔥 🔥 
> ( > ) Maior que
>( < ) Menor que
>( >= )  Maior ou igual a
>( <= )  Menor ou igual a
>( = ) Igual a
>( <> )  Diferente de

### Comentários🔥 🔥 

> //  Linha de Comentário
> {} Texto de Comentário - várias linhas
