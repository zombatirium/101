HOTCODE
    compilador compila para código de máquina, quando nota que algo está sendo muito usado

arquivo -> compilador -> assembly
               |
     ---------- 
     |
|FRONT-END|                    x86
|    c    |                   /
|    Go   |   -> IL -> BACKEND -- x64
|    Rust |                   \
                              ARM


FRONT-END -> como lê o arquivo (gera IL)
IL -> linguagem intermediária
BACKEND -> para arquitetura

Python compila (para IL) e VM interpreta bytecode

IL -> VM <--> Real Machine


Compilador Rust,go,c -> compila para Real Machine (x86, x84, ARM)
Compilador do Python -> compila para VM (máquina que não existe)

[Como o interpretador do Python funciona？ ｜ Live de Python #218](https://youtube.com/watch?v=pxfZTAJDipY)
