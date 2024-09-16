### AVANÇANDO NA PROGRAMAÇÃO

A ideia deste módulo é justamente essa: mostrar a você como é possível armazenar mais de um valor em uma mesma estrutura (que agora, perde o nome de variável). Essas estruturas pertencem a um grupo computacional conhecido como estruturas de dados.

Essas estruturas de dados são componentes computacionais que manipulam os dados e realizam operações entre a memória e o processador. Existem alguns tipos de estruturas de dados, mas aqui trataremos especificamente da estrutura conhecida como “vetor” e sua subcategoria, a matriz.

É importante ressaltar o seguinte: nenhuma linguagem de alto nível possui, de fato, vetores. O termo “alto nível” refere-se à distância entre o código digitado pelo programador e o código de máquina interpretado pelo computador (código Assembly - que ainda é legível a humanos, mas muito mais próximo de uma leitura computacional). Logo, as linguagens são basicamente divididas entre alto nível ou baixo nível e o código que todo programador escreve é, inevitavelmente, de alto nível.

Os vetores, por exemplo, são estruturas de dados que lidam diretamente com endereço de memória, realizando alocação de dados em endereços específicos. Algumas linguagens, como C, simulam um acesso direto à memória, mas ainda existe uma camada intermediária entre o código digitado e a memória física.

Desta forma, pode-se afirmar corretamente, considerando que os vetores têm acesso direto ao hardware da máquina (regidos pelo Kernel do Sistema Operacional), que nenhuma linguagem de alto nível trabalha, efetivamente, com vetores ou matrizes, mas sim, com objetos que simulam um vetor ou matriz.

Todos esses tipos de objeto que simulam um vetor ou uma matriz, possuem algumas características:

Armazenam um ou mais valores;
Os valores podem ser numéricos ou textuais (caracteres);
Cada valor é armazenado em um índice numérico sequencial;
Os índices sempre inicial na posição 0;
As listas em Python são heterogêneas, ou seja, podem conter elementos de diferentes tipos.

---

### CONCEITO DE TUPLAS

Uma tupla é representada em Python como uma “sequência de valores separados por vírgulas” (Python.org) por um conteúdo envolto em parênteses.

a = (1,2,3)

Neste exemplo já não chamaremos o “a” de variável, mas sim, de tupla, uma vez que ela tem vários valores atrelados.

O valor inserido na tupla pode ser resgatado apontando-se o endereço do índice 

a = (1,2,3)
print(a[0])

Para facilitar, você pode sempre pensar que o índice desejado sempre terá a grandeza n-1 em relação à quantidade de elementos em sua tupla, por exemplo, se você quiser resgatar o terceiro elemento de uma tupla, o índice será a posição n-1, ou seja, 3-1 (posição 2).
Dentro do Python, não utilizamos as palavras vetor e matriz, mas sim de alguns termos, como lista.

É possível trabalhar com alguns comandos específicos do Python para fazer uma varredura nas estruturas de dados. Neste caso, utilizaremos um comando que irá “varrer” a tupla em busca de um valor específico:

tupla = (1,2,3,4,5)
if 8 in tupla:
    print("existe)
else:
    print("não existe")

Neste exemplo, utilizamos uma condicional (if) para verificar se o valor 18 estava presente dentro da tupla nomeada como “tupla”. Como o valor não está presente, o bloco de execução que será ativado será aquele disposto na linha 316, o else.

Lista é um dos modelos que utilizamos na hora de fazer vetorização ou matrizes dentro da programação em Python.

O segundo modelo que veremos é o conceito de tuplas.

Tuplas são bem similares às listas, é a possibilidade que você tem de colocar um conteúdo dentro de uma variável para que essa variável consiga armazenar uma sequência de valores.

É diferente de uma variável convencional, em que você consegue alterar o valor tirando a informação antiga da caixinha e colocando uma nova.

Já no conceito de lista não, pois você consegue adicionar vários valores dentro da lista.

E conseguimos também chamar um elemento específico da lista.

CHAMANDO O ELEMENTO ZERO, NO CASO O NÚMERO 1:

a = [1,2,3]

print(a[0])

---

Conseguimos também trabalhar com alguns recursos:

ADICIONANDO UM NOVO ELEMENTO:

a = [1,2,3]
a.append(4)
print(a)

---

A ÚNICA DIFERENÇA DA TTUPLA E DA LISTA É QUE A TUPLA É IMUTÁVEL (É ALGO QUE NÃO MUDA) E A LISTA É MUTÁVEL.

NÃO CONSEGUIMOS RETIRAR E NEM COLOCAR UM ELEMENTO, NEM EXPANDIR A TUPLA POSTERIORMENTE.

---

ALGUMAS OPERAÇÕES QUE CONSEGUIMOS FAZER COM TUPLAS E LISTAS:

O RECURSO in VEREIFICA SE UM ELEMNTO PERTENCE A UMA LISTA, TUPLA, DICIONÁRIO OU CONJUNTO.

tupla = (1,2,3,4,5,6,7,8,9,0)
if 8 in tupla:
     print("Existe")
else:
     print("

E podemos fazer buscas em um banco de dados, como por exemplo se existir eterminado número de telefone no banco de dados, ligue para ele.

---

### LISTAS

Seguindo a mesma lógica das tuplas, temos as listas. Elas seguem o princípio de “pilhas” em que o item adicionado por último é o primeiro a ser recuperado, mas nada impede que elas também sejam utilizadas como filas, em que o último item adicionado é também o último a ser retirado (Python.org).

Basicamente existem duas diferenças entre as listas e as tuplas:

Tuplas são imutáveis, listas não
Tuplas utilizam parênteses, listas utilizam colchetes

a = [1,2,3]

ALGUMAS MANEIRAS DE MANIPULAR LISTAS:

a.append(4)
a.remove(2)
a.insert(0, 50)

---

### CONCEITO DE DICIONÁRIOS

Um dicionário se comporta da mesma forma que uma lista ou tupla; na verdade, o que os difere é mais uma questão conceitual e de usabilidade, uma vez que o dicionário de dados vai nomear cada índice, de forma que seja mais fácil memorizar seus respectivos valores.

Imagine uma lista com os dados do cadastro de um usuário com as informações mais ou menos desta forma:

cadastro = [“João”, “Silva”, 34, “45454545”, “33333333333”, “Alameda dos Golfinhos”, “SP”, 12122222”]

Convenhamos que memorizar em qual índice está alocado o CPF do usuário é algo um tanto complicado, afinal, são tantas informações que é até normal se confundir em meio aos dados. Não seria bem mais útil se cada campo, ao invés de um índice, tivesse como referência uma palavra que o identificasse? Pois é, é justamente esse o conceito de dicionários.

Com os dicionários de dados, uma estrutura do tipo “vetor” (note as aspas) passa a ter nomes ao invés de índices, facilitando a sua manipulação por meio da memorização. Isso é demonstrado em detalhes na Figura 42 (desconsidere a forma como o código foi escrito; esta apresentação foi apenas para que a linha não ficasse muito extensa).

Observe que, na linha 371, ao ser requerido o valor “cpf” (inicialmente apontado na linha 368), o resultado “33333333333” foi impresso na tela sem que houvesse a necessidade de se utilizar um índice numérico.

cadastro{
         "nome" : "Rafaela",
         "cpf" : "43554186856",
         "idade" : 24
         }
print(cadastro["cpf"])

DICIONÁRIO: É UMA LISTA DE VALORES, MAS AO INVÉS DE VOCÊ TER ÍNDICES OCULTOS E NÚMERICOS, VOCÊ TERÁ INDICES QUE SÃO MUITO MAIS AMIGÁVEIS DE FORMA TEXTUAL.

SE EU TIVER 50 ITENS NA MINHA LISTA, NÃO LEMBRAREI DE CABEEÇA QUAL O ÍNDICE 47.

O DICIONÁRIO TRABALHA EM CIMA DE LISTAS E TUPLAS ATRIBUINDO NOMES A CADA ÍNDICE.

PARA TER UMA LISTA EM FORMA DE DICIONÁRIO, TEREI QUE CRIAR UM ÍNDICE TEXTUAL QUE IRÁ CORRESPONDER A UM VALOR SEJA ELE TEXTUAL OU NUMÉRICO.

lista = {"nome" : "Marcio", "sobrenome" : "Santos"}
print(lista["nome"], lista["sobrenome"])

ISSO É MUITO UTILIZADO PRINCIPALMENTE QUANDO TRABALHADO COM ANÁLISE DE DADOS, POIS QUANDO VOCÊ ESTÁ TRABALHANDO COM ANÁLISE DE DADOS VOCê TEM O PROCESSO DE ETL(EXTRACT, TRANSFORM, LOAD), VOCê EXTRAI OS DADOS DE ALGUM LUGAR/BANCO DE DADOS/ARMAZÉM DE DADOS, TRANFORMA ESSA INFORMAÇÃO E CARREGA UMA NOVA ESTRUTURA PARA PODER FAZER A ANÁLISE. E O PROCESSO DE TRANFORMAÇÃO DO ETL UTILIZA ESSE TIPO DE ESTRUTURA, POIS DIFICILMENTE VOCê CONSEGUIRÁ PUXAR UMA INFORMAÇÃO E TRABALHAR COM ÍNDICES NUMÉRICOS, COMO SÃO MUITOS ÍNDICES, É MAIS COMPLICADO MEMORIZAR ELES.

---

### CONCEITO DE CONJUNTOS

A lógica de conjuntos é a mesma que aplicamos às listas ou tuplas mas com uma característica peculiar: ela não possui elementos repetidos. Seu caractere de marcação é um par de chaves. De acordo com a documentação oficial do Python, os conjuntos são

“uma coleção desordenada de elementos, sem elementos repetidos. Usos comuns para conjuntos incluem a verificação eficiente da existência de objetos e a eliminação de itens duplicados. Conjuntos também suportam operações matemáticas como união, interseção, diferença e diferença simétrica.” (Python.org).

a = {1,2,3,3,3,3,4,5,5,5,6,1}
print(a)

{1,2,3,4,5,6}

Uma série de recursos também é possível de ser realizada com os conjuntos, como por exemplo, descobrir uma intersecção (elementos comuns) entre conjuntos, elementos destoantes, elementos presentes apenas em um dos conjuntos, etc. Na Figura 40 é possível como funcionaria essa lógica aplicando o recurso de intersecção, ou seja, a descoberta apenas de elementos comuns a dois conjuntos. O resultado impresso em tela seria: 1,2,3

a = {1,2,3,4,5,1,1,2,3,2,2}
b = {1,2,3}
c = a.intersection(b)
print(c)

Conjunto é uma estrutura padrão que você aplica em vetores ou matrizes (ou seja, você aplica em uma lista, tupla ou dicionário)

E lembrando que o dicionário é apenas uma forma diferenciada de você trabalhar com conceito de lista ou tupla, não é um subtipo, mas sim uma forma de trabalho, assim como o conjunto.

COMO ACHAR O PONTO DE INTERCECÇÃO ENTRE ESSES DOIS ELEMNTOS/ESSAS DUAS LISTAS:

PARA APONTAR QUE ESTAMOS TRABALHANDO COM CONJUNTO, USAMOS A PALAVRA RESERVADA SET.

a = {1,3,5}
b = {2,4,6}

print(set(a.intersection(b)))

O PROGRAMA NOS RETORNARÁ set() POIS NÃO EXISTEM ELEMNETOS QUE ESTÃO PRESENTES NA INTERSECÇÃO ENTRE O A E O B.

Um Diagrama de Venn usa círculos sobrepostos ou outras formas para ilustrar as relações lógicas entre dois ou mais conjuntos de itens. Muitas vezes, eles servem para organizar graficamente as coisas, destacando como os itens são semelhantes e diferentes.

Intercecção é o espaço que está presente tanto no conjunto A quanto no conjunto B.

EXISTEM OUTRAS FOPRMAS DE TRABALHAR COM DIAGRAMA DE VENN:

VERIFICANDO APENAS OS ITENS QUE ESTÃO PRESENTES NO CONJUNTO A.

OU APENAS NO CONJUNTO B.

OU OS ITENS PRESENTES NO CONJUNTO A, B E QUE NÃO ESTÃO PRESENTES NOPS DOIS AO MESMO TEMPO (A INTERCECÇÃO FICA DE FORA).

print(set(a.difference(b)))
print(set(a.symmetric_difference(b))) PERTENCE SÓ A UM DOS SUBCONJUNTO
print(b.issubset(a))

---

### TUPLAS E CONJUNTOS EM CASOS REAIS

Vou criar uma lista (lista = []), um laço de repetição (for), uma variável de controle (a), um intervalo de 5 posições (range(5)), vou dizer que a minha lista vai adicionar algum elemento no final da sua estrutura e esse elemento será do tipo input permitindo que a pessoa digite um nome e iremos printar a lista.

lista = []

for a in range(5):
    lista.append(input("Nome: ")

print(lista)

---

### OTIMIZAÇÃO DE TUPLAS

Resumindo, temos algumas estruturas padrões, que conseguimos utilizar quando vamos fazer vetor ou matriz, utilizando listas ou tuplas, facilitando a estrutura através de dicionários, e também conseguindo fazer algumas operações extras utilizando conjuntos.

---

### TESTANDO A EFICIÊNCIA DOS CÓDIGOS
















