Análise de Complexidade Ciclomática
é uma métrica de software 
que avalia os possíveis caminhos de um algoritmo

Criada por Thomas McCabe e divulgada em 1976
num artigo chamado
A Complexity Measure - Uma medida de complexidade

No qual, McCabe propõe a criação de um grafo
para analisar os possíveis trajetos do algoritmo
e daí avaliar sua complexidade

Os possíveis nós para a criação do grafo, são
todos os elementos que vão utilizar de lógica
para decidir o caminho:
    * if
    * else if
    * swith 
        1. case -> nó
        2. case -> nó
    * while
    * do while
    * try cat

Métodos de Cálculo da Complexidade Ciclomática
    1. contar a quantidade de regiões do grafo da complexidade ciclomática
    2. V(G) = E - N + 2
       * V(G) -> número ciclomático
       * E    -> número de arestas
       * N    -> número de nós
    3. V(G) = P + 1
       * V(G) -> número ciclomático
       * P    -> número de componentes (ou comandos de desvio -> else)

    EX:
        ```
            bool verifica_idade(int idade_pessoa) {
                if (idade_pessoa >= 18)
                    return true
                else
                    return false
            }
        ```

        ```
        ┌────────┐     ┌────┐        R2        ┌───────┐        ┌─────┐
        │ inicio │ ─── │ if │ ──────────────── │ endif │ ────── │ fim │
        └────────┘     └────┘        R1        └───────┘        └─────┘
                         │        ┌──────┐         │
                         └─────── │ else │ ────────┘
                                  └──────┘

        ```

        1. contar a quantidade de regiões do grafo da complexidade ciclomática
            ANÀLISE:
                R1 -> região fechada
                R2 -> região externa

                R1 + R2 = 2

        2. V(G) = E - N + 2
            ANÀLISE:
                E -> número de arestas (linhas) = 5
                N -> número de nós              = 5
 
                V(G) = 5 - 5 + 2 
                V(G) = 0 + 2 
                V(G) = 2

        3. V(G) = P + 1
            ANÀLISE:
                P -> número de componentes (ou comandos de desvio -> else) = 1

                V(G) = 1 + 1 
                V(G) = 2
 

# REFERÊNCIAS
[A Complexity Measure](https://www.literateprogramming.com/mccabe.pdf)
[Complexidade Ciclomática - Conceitos e Cálculo da Métrica (Grafo)](https://youtube.com/watch?=XuOSbbFTgGA)
[Complexgraph](https://code.google.com/p/complexgraph/downloads/list)
[Golang - Análise de complexidade ciclomática](https://github.com/fzipp/gocycl)
[Rust - complexidade ciclomática](https://docs.rs/complexity/latest/complexity/)
[Treinaweb - complexidade ciclomática análise estática e refatoração](https://www.treinaweb.com.br/blog/complexidade-ciclomatica-analise-estatica-e-refatoracao)
