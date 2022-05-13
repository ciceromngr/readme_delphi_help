# Primeiro programa em delphi 

- Criacao de classes
  - type TNomeClasse = class
  - Atributos: NomeAtributo : Tipo (pode ser string, integer, etc...)
  - Methods: procedure NomeDoMetodo, Lembrando que esse procedure ele é uma funcao void
  - no implementation inicializar os methods : 
  
         procedure TNomeClasse.NomeDoMetodo; 
         begin
         end;
  
  - A unit é um local onde são agrupados as funções e os procedimentos de maneira que possam vir a ser utilizados pelo programa principal. Além dessas três partes, o código poderá ter a chamada initialization e finalization que são opcionais 
  - Unit exemplo:
                
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
