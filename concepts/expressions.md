### Expressões

Todo o código Common Lisp é feito de S-Expressions (Symbolic Expressions. Eles são chamados de sexprs para ser breve. Cada sexpr é um átomo ou um contras. Quando as expressões S são avaliadas, elas retornam automaticamente algum valor que toma o lugar da expressão. Ao escrever suas próprias funções (usando defun), o último valor dentro do corpo de defun é retornado automaticamente:

```lisp
;; Defining a new function
(defun gimme-foo () 'foo)
;; Calling the function as an S-Expression
(gimme-foo) ; => FOO