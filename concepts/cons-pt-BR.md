### Contras

Todo o código Common Lisp é um "átomo" (um valor único e indivisível) ou uma lista (também chamada de "contras"). Um contras é composto por duas partes: o primeiro elemento e o resto dos elementos. Por razões históricas, essas duas partes são chamadas de `car` e de `cdr`. Quando esses itens são avaliados como código, o primeiro elemento (`car`) representa a função que está sendo chamada, enquanto o resto dos elementos (`cdr`) representam os argumentos dessa função:

```lisp
(<function> <arg1> <arg2> ... <argN>)
; ^ car ^  |        ^ cdr ^
