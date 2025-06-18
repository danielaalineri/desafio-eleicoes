# Java Vote Counter from File

Este é um programa Java simples que lê um arquivo de texto contendo nomes e quantidades de votos (formato CSV) 
e gera um relatório com o total de votos por candidato.

## 🗳️ Funcionalidade

- Solicita ao usuário o caminho completo de um arquivo `.txt` ou `.csv`.
- Lê cada linha do arquivo no formato:
- Nome,Quantidade (por exemplo: Maria,10)
- Ou seja, cada linha contém o nome de um candidato seguido da quantidade de votos recebidos, separados por vírgula.
- Armazena os dados em um `LinkedHashMap` para manter a ordem de inserção.
- Exibe o total de votos de cada candidato no terminal.

## 🧾 Exemplo de Arquivo de Entrada (`votes.txt`)
Alex,5
Maria,10
Bob,3
Maria,2
Alex,4
> *⚠️ Atualmente, o programa **não acumula** votos repetidos. Ele sobrescreve se o nome já existir.*

## 💻 Exemplo de Execução

```text
Enter file full path: 
C:\Users\Daniela\Documents\votes.txt
Alex: 5
Maria: 10
Bob: 3

📂 Estrutura

src/
└── app/
    └── Program.java

📚 Conceitos Utilizados

    Leitura de arquivos com BufferedReader e FileReader

    Uso de Map<String, Integer> (neste caso, LinkedHashMap) para armazenar pares nome → votos

    Manipulação de arquivos CSV simples

    Estrutura de repetição com while e controle de exceções com try-with-resources

🛠️ Como Executar

    Compile o programa:

javac app/Program.java

Execute:

    java app.Program

    Insira o caminho completo de um arquivo .txt com os votos.

👩‍💻 Autora

Daniela Alineri
Projeto criado para praticar leitura de arquivos e uso de mapas (Map) em Java.

