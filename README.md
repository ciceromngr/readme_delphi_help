# README Delphi Helpers 🚀🚀🚀🚀

- Criacao de classes 🔥 🔥 
  - > type TNomeClasse = class🔥 🔥 
  - > Atributos: NomeAtributo : Tipo (pode ser string, integer, etc...)🔥 🔥 
  - > Methods: procedure NomeDoMetodo, Lembrando que esse procedure ele é uma funcao que não tem retorno ou seja void🔥 🔥 
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

### Operadores Relacionais  🔥🔥 
> ( > ) Maior que

>( < ) Menor que

>( >= )  Maior ou igual a

>( <= )  Menor ou igual a

>( = ) Igual a

>( <> )  Diferente de

### Comentários 🔥🔥 

> //  Linha de Comentário

> {} Texto de Comentário - várias linhas

### Condicionais 🔥🔥

> if

    if (condição) then
      begin
        {Bloco de comandos executados se a condição for verdadeira}
      end
    else
      begin
        {Bloco de comandos executados se a condição for falsa}
    end;

> If encadiado

    if (condição) then
      begin
        {Bloco de comandos executados se a condição for verdadeira}
      end
    else if (condição) then
      begin
          {Bloco de comandos executados se a primeira condição for falsa e está condicao for verdadeira}
      end
    else
      begin
        {Bloco de comandos executados se a condição for falsa}
    end;
### Obs .:
  > begin e o end são opcionais case ouver uma unica instrução de codigo

    if (condição) then
        {comando executado se a condição for verdadeira}
    else
        {comando executado se a condição for falsa};
> if not then

    if not (false) then
      begin
        {Bloco de comandos executados se a condição for verdadeira}
      end
    else
      begin
        {Bloco de comandos executados se a condição for falsa}
    end;

### Referências com o Comando With 🔥🔥
> O with é como se fosse um comando de leitura e pode ser usado assim:

    with Query1 do
      begin
      Close;
      SQL.CLear;
      SQL.Add(´Select * from CLientes´);
      Open;
    end;

> do contario vc teria que fazer assim:

    Query1.Close;
    Query1.SQL.CLear;
    Query1.SQL.Add(´Select * from CLientes´);
    Query1.Open; 

> para varrer e setar propriedades dos componentes.

- Uso sem with num memo

      memo1.clear;
      memo1.loadfromfile('');
      memo1.lines.add('teste1');

- Uso com with num memo

      with memo1 do 
      begin
        clear;
        loadfromfile('');
        lines.add('teste1');
      end;

### Loops 🔥🔥
> for - to - crescente

    var I : Integer;
    begin
      for I := 0 to 100 do
      begin
        {Bloco a ser executado até o fim do loop}
      end;
    end;
> for - DownTo - decrecente

    var I : Integer;
    begin
      for I := 100 DownTo 0 do
      begin
        {Bloco a ser executado até o fim do loop}
      end;
    end;

> While do


    var
      i : Integer;
      message: String;
    begin
      i := 0;

      while i < 10 do
      begin
        if (i mod 2 = 0) then
        begin
          message := 'O valor ' + i.ToString() + ' é par! ';
          ListBox1.Items.Add(message);
          inc(i);
        end
        else
          begin
            message := 'O valor ' + i.ToString() + ' é Impar! ';
            ListBox1.Items.Add(message);
            inc(i);
          end;
      end;
    end;

> repeat until

  > - obs :. Para quem vem de outras linguagens o reapeat until seria o mesmo que : do while

    outras linguagens:.
      do {
        // o bloco de comandos deve se executado pelo menos 1 vez
      } while ( condicao ); 
      // Se a condicao for verdadeira o bloco de codigo e repetido

>

    Delphi  :.
    var
      i : Integer;
      message: String;
    begin
      i := 0;

      repeat
        // o bloco de comandos deve se executado pelo menos 1 vez
        if (i mod 2 = 0) then
          begin
            message := 'O valor ' + i.ToString() + ' é par! ';
            ListBox1.Items.Add(message);
            inc(i);
          end
        else
          begin
            message := 'O valor ' + i.ToString() + ' é Impar! ';
            ListBox1.Items.Add(message);
            inc(i);
          end;
      until ( i > 10 ); //condicao false o bloco é executado novamente
      // Preste atencao enquanto o codigo for false ele continua a execucao
      // 😏 é diferente do tradicional do while que enquanto for verdade o codigo repete  
    end;
