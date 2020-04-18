# CURSO DE SASS

## Interface online
* https://www.sassmeister.com/
* Dentro da interface temos a possibilidade de modificar o tipo de saida

## Modificando tipo de saída
* $ sass [Nome do Arquivo SCSS] [Nome do Arquivo CSS] --style [Tipo de Saida(nexted, expanded, compact, compressed)]
* $ sass --watch [Pasta Sass Que será monitorada]:[Pasta CSS que terá os CSS Compilados] --style [Tipo de Saida(nexted, expanded, compact, compressed)]
* Comentário para aparecesser em arquivo minificado /*! texto */

## Shel Interativo do SassScript
* sass -i (comando para utilizar o shel do sass no terminal)
* Tipos de dados
    * Mapa de dados:
        $mapa = (campo1:valor, campo2:valor);
        $cor = mapa-get($mapa, campo1);
    * Type-of(Identificar tipo da váriavel):
        type-of($mapa); 

## Imports no Sass
* @import 'nome do arquivo com ou sem extensão';

## Arquivo Partials
* deve ser colocado um (_) na hora da sua criação.
* Arquivos utilizados para pequenas ações de fatoração e não é processado pelo sass mas é possivel importação

## Mixins(Funções do Sass) 
* São utilizados no mesmo conceito de funções afim de padronizar e ajudar o na padronização de algumas tarefas.
* Dentro do arquivo de style.scss tem alguns exemplos.

## Extends(Extenções de classe)
* São utilizados com a mesma caracteristica de uma classe e aonde dentro de um componente pode ser
feito a extenção, podendo ser num conseito de classe(Orientação objeto) ou num conceito de class ou id do próprio css.
* Para criar um extend no conceito de classe orientada a objeto é necessário o caracter (%) na frente e o nome técnico dele é placeholder
* Dentro do arquivo de style.scss tem alguns exemplos.

## Operações
* Verificar no ppt de operações para dúvidas
* Função de hsl para construir cores colocando hsl(cor, tonalidade, e luminosidade) exemplo:
    color: hsl(0, 100%, 50%) // vermelho
* Existem também outras funções para atacar uma função expecifica
    * clareando cor lighten, exemplo:
        color: lighten(read, 50%) // vermelho
    * escurecendo cor darken, exemplo:
        color: lighten(read, 50%) // vermelho
    * modificando a saturação cor saturate, exemplo:
        color: saturate(read, 50%) // vermelho    
    * diminuir a saturação cor desaturate, exemplo:
        color: desaturate(read, 50%) // vermelho  
    * alterar a tonalidade de cor adjust-hue, exemplo:
        color: adjust-hue(read, 50%) // vermelho  