### Instruções

Você! Sim você, corajoso ouvinte! Lenny, o alienígena ceceio, precisa da sua ajuda! Lenny quer sair com todos os outros alienígenas ceceios, mas seus pais disseram a Lenny que eles não vão a lugar nenhum até que o quarto esteja limpo.

O problema é que Lenny mal consegue ver o chão! Lenny não consegue diferenciar seus átomos de seus contras, seus símbolos de suas palavras-chave, seus `cars` de seus `cdrs`!

Você pode ajudar Lenny a resolver essa bagunça? Não se esqueça dos **parênteses** , você vai precisar deles!

### 1. Atualize Lenny nos símbolos
Antes que Lenny possa começar, eles precisam de uma atualização sobre como são os símbolos e palavras-chave - já faz um tempo desde a última vez que eles foram organizados ... Ajude Lenny definindo duas funções: `lennys-favorite-foodque` avalia para algum símbolo e `lennys-secret-keywordque` avalia para alguma palavra-chave . Por exemplo:

```lisp
(lennys-favorite-food) ; => LASAGNA
```
```lisp
(lennys-secret-keyword) ; => :ALIENS-ARE-REAL
```
Observe que você pode retornar qualquer símbolo ou palavra-chave que desejar (se não for fã de lasanha ou se não acreditar em alienígenas).

### 2. Ajude Lenny a distinguir entre átomos e contras
Depois que Lenny tiver revisado os símbolos e palavras-chave, é hora de começar a limpar! Para classificar todas as expressões S espalhadas pela sala, Lenny precisa de ajuda para determinar o que é um contras e o que é um átomo. Você pode ajudar implementando duas funções `is-an-atom-p` e `is-a-cons-p`:

```lisp
(is-an-atom-p 'one-thing)    ; => T
(is-an-atom-p '(two things)) ; => NIL
```
```lisp 
(is-a-cons-p 'one-thing)    ; => NIL
(is-a-cons-p '(two things)) ; => T
```

Para esta seção, há várias funções integradas de lisp que podem ser úteis. Além disso, por enquanto, você pode simplesmente considerar `T` como verdadeiro e `NIL` como falso.

### 3. Ajude Lenny a dividir seus contras
Finalmente, as consolas de Lenny são muito volumosas para serem guardadas com cuidado, então eles precisam dividi-las em partes menores. Você pode ajudar definindo mais duas funções para quebrar seus contras ( `first-thing` e `rest-of-it`)?

```lisp
(first-thing '(first second third)) ; => FIRST
(rest-of-it  '(first second third)) ; = (SECOND THIRD)
```

Novamente, algumas das funções integradas do Common Lisp podem ser úteis aqui.