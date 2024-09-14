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

Dentro do Python, não utilizamos as palavras vetor e matriz, mas sim de alguns termos, como lista.

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

### CONCEITO DE DICIONÁRIOS

DICIONÁRIO: É UMA LISTA DE VALORES, MAS AO INVÉS DE VOCÊ TER ÍNDICES OCULTOS E NÚMERICOS, VOCÊ TERÁ INDICES QUE SÃO MUITO MAIS AMIGÁVEIS DE FORMA TEXTUAL.

SE EU TIVER 50 ITENS NA MINHA LISTA, NÃO LEMBRAREI DE CABEEÇA QUAL O ÍNDICE 47.

O DICIONÁRIO TRABALHA EM CIMA DE LISTAS E TUPLAS ATRIBUINDO NOMES A CADA ÍNDICE.

PARA TER UMA LISTA EM FORMA DE DICIONÁRIO, TEREI QUE CRIAR UM ÍNDICE TEXTUAL QUE IRÁ CORRESPONDER A UM VALOR SEJA ELE TEXTUAL OU NUMÉRICO.

lista = {"nome" : "Marcio", "sobrenome" : "Santos"}
print(lista["nome"], lista["sobrenome"])

ISSO É MUITO UTILIZADO PRINCIPALMENTE QUANDO TRABALHADO COM ANÁLISE DE DADOS, POIS QUANDO VOCÊ ESTÁ TRABALHANDO COM ANÁLISE DE DADOS VOCê TEM O PROCESSO DE ETL(EXTRACT, TRANSFORM, LOAD), VOCê EXTRAI OS DADOS DE ALGUM LUGAR/BANCO DE DADOS/ARMAZÉM DE DADOS, TRANFORMA ESSA INFORMAÇÃO E CARREGA UMA NOVA ESTRUTURA PARA PODER FAZER A ANÁLISE. E O PROCESSO DE TRANFORMAÇÃO DO ETL UTILIZA ESSE TIPO DE ESTRUTURA, POIS DIFICILMENTE VOCê CONSEGUIRÁ PUXAR UMA INFORMAÇÃO E TRABALHAR COM ÍNDICES NUMÉRICOS, COMO SÃO MUITOS ÍNDICES, É MAIS COMPLICADO MEMORIZAR ELES.

---

### CONCEITO DE CONJUNTOS

Conjunto é uma estrutura padrão que você aplica em vetores ou matrizes (ou seja, vocÊ aplica em uma lista, tupla ou dicionário)

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











