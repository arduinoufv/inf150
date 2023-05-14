Executavel do espresso no colab já compilado

foi gerado com os comandos

```
!git clone https://github.com/classabbyamp/espresso-logic.git
%cd espresso-logic/espresso-src
!make >& /dev/null
%cd ../..
!cp espresso-logic/bin/espresso .
```
