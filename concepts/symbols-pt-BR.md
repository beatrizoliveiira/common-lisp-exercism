### Símbolos

Os símbolos em Common Lisp são valores especiais que podem apontar para outros valores ou, no caso de palavras-chave , eles próprios. Quando os símbolos são avaliados pelo Lisp, eles são substituídos pelos valores para os quais eles apontam:

```lisp
foo  ; => <whatever-foo-points-to>
:foo ; => :FOO
```
Observe que as palavras-chave são denotadas por dois pontos (`:`).

Aspas - a adição de 'antes de uma expressão S - diz ao Lisp para não avaliar essa expressão. Citando 'fooem nosso defunexemplo, evitamos que Lisp tentasse procurar (e não conseguisse encontrar) o que FOOdeveria apontar para, em vez disso, retornar o FOOpróprio valor . Se FOOnão foi definido em nenhum lugar em nosso programa:

```lisp
foo  ; => <ERROR! Lisp doesn't know what foo points to!>
'foo ; => FOO
```

Por enquanto, você pode considerar isso apenas como uma forma de retornar símbolos de uma função.