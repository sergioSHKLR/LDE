<script src="https://hypothes.is/embed.js" async></script>

# 👻 O Livro dos Espíritos

1️⃣ Primeiro sub *repo* de [doutrina.org](https://github.com/sergioSHKLR/doutrina.org), *hosted* no Github.

## Direto ao ponto                       

- 📔 [LDE-2023-07-14.md](./releases/LDE-2023-07-14.md)

### Formatação de texto (livro impresso)

Como exemplificado abaixo (trecho intencionalmente modificado do original), a editora usou a divisão visual (linhas em branco; aspas) e estilística (fonte normal; itálico; fonte menor) para separar elementos (origem humana; origem espiritual) e denotar realce ou grifo. 

#### Questões (livro impresso)

Como se vê, na pergunta, a palavra **Deus** foi realçada em estilo normal, visto que a sentença se encontra em estilo itálico. Já na resposta, palavra **insuficiente** foi realçada em estilo itálico, visto que a sentença se encontra em estilo normal. De modo a diferenciar os comentários de Kardec das mensagens de Espíritos, usou-se uma fonte ligeiramente menor em tamanho.

---

<span style="font-family: serif;">
<b>3.</b><span style="font-style: italic; margin-left: 30px;">Poder-se-ia dizer que <span style="font-style: normal">Deus</span> é o infinito?</span></span><br />

<p style="font-family: serif; margin-left: 40px;">“Definição incompleta. Pobreza da linguagem humana, <i>insuficiente</i> para definir o que está acima da linguagem dos homens.”</p>

<span style="font-family: serif; margin-left: 70px; font-size: 90%;">Deus é infinito em suas perfeições, mas o infinito é uma abstração. Dizer que Deus é o <i>infinito</i> é tomar o atributo de uma coisa pela coisa mesma, é definir uma coisa que não está conhecida por uma outra que não o está mais do que a primeira.</span>

---

#### Trechos bíblicos

Trechos bíblicos, em geral, não foram separados ou atribuídos por livro, capítulo e versículo.

---

<p style="font-family: serif; width: 100%;">E disse Jesus: “A cada um, de acordo com suas obras.”</p>

---

Consideramos estas escolhas de formatações demasiada sutis (não chamam a atenção do leitor com eficiência), além de introduzir dificuldades na padronização programática. Adicionalmente, as mesmas não são apropriadas para a análise e formatação automática por meio de *scripts*, sendo o método que nosso maior colaborador, **<a href="https://github.com/JhonnyBn">JhonnyBn</a>**, criou para automatizar parte de nosso processo.

## Método

Em primeiro lugar, teríamos que estabelecer padrões de divisão, hierarquia, e formatação de texto que mantivessem a fidelidade ao original, não em forma, mas em conteúdo.

Analisando a divisão do livro em partes, decidimos criar uma seção anterior à `LDE-1` 🗂️ Parte 1 como `LDE-0` 🗂️ Parte 0, e dar-lhe o título de Pré-textual. Similarmente, criamos uma seção posterior à `LDE-5` 🗂️ Parte 5, e por dar-lhes o nome de `LDE-6` 🗂️ Parte 6 e o título de Pós-textual.

## Padrões

### Livros

Individualmente, iremos identificar os livros pelos emojis e/ou siglas abaixo.

| **Emoji** | **Sigla** | **Livro** |
|---|---|---|
| 👻 | `LDE` | O Livro dos Espíritos |
| ✒️ | `LDM` | O Livro dos Médiuns |
| 🕊️ | `ESE` | O Evangelho segundo o Espiritismo |
| 🔥 | `CEU` | O Céu e o Inferno |
| 🌱 | `GEN` | A Gênese |

### Hierarquia

Dentro deste livro, usaremos os emojis abaixo para identificar elementos individuais ou grupamentos dos mesmos. Note também o correspondente código mestre.

<pre>
📔 livro
 |
 └── 🗂️ parte
      |
      └── 📑 capítulo
           |
           └── 📃 seção
                |     
                └── #️⃣ questão
</pre>

Para facilitar a organização hierárquica, localização, correlação de items, e brevidade, um código chave foi criado. Para isso, pequenas mudanças foram feitas ─ em forma, não em conteúdo. Este código alfanúmerico é demonstrado abaixo.

### Código chave

<pre>
LDE-X-XX-XX
 |  |  |  |
 |  |  |  └── 📃 seção
 |  |  | 
 |  |  └── 📑 capítulo
 |  |
 |  └── 🗂️ parte
 |
 └── 📔 livro
</pre>

E em especial no LDE, o código para questões é modificado da sequência lógica de `LDE-X-XX-XX-XXXX` para:

<pre>
LDE-qXXXXa
 |   |   |
 |   |   └── sub-questão
 |   |
 |   └── #️⃣ questão
 |
 └── 📔 livro
</pre>

Como ilustrado acima, usamos três letras para o livro, um dígito para partes, e dois dígitos para capítulos e itens. Em especial, no LDE, usamos a letra `q`, de um a quatro dígitos, e uma letra minúscula para sub-questões de modo a designar uma pergunta específica (ex. `LDE-q909a`).

Em suma, temos esta tabela descritiva abaixo:

| **Emoji** | **Descrição** | **Conteúdo** | **Código chave** |
|---|---|---|---|
| 📔 | livro | obra completa | `LDE` |
| 🗂️ | parte | subdivisão da obra | `LDE-X` |
| 📑 | capítulo | subdivisão de partes | `LDE-X-XX` |
| 📃 | seção | subdivisão de capítulos | `LDE-X-XX-XX` |
| #️⃣ | questão | pergunta, reposta e comentário * | `LDE.qX` |

/* Existem exceções deste formato, tais como 59, 100-113, 222, 257, 455 e 872.

**Adicionais**

| **Emoji** | **Descrição** | **Conteúdo** |
|---|---|---|
| :latin_cross: | trecho bíblico | trecho atribuído com livro, capítulo e versículo |
| :point_right: | segmento relacionado | indicação para leitura complementar |

<!--
| 🗃️ | Índice Geral | coleção de 🏷️ _tags_ |
| 🏷️ | _tag_ | agrupa #️⃣ questões e/ou 📃 seções por assunto |
| ⚜️ | fim | término de um elemento | 
-->

## Padrões estabelecidos

Decidimos utilizar um tipo *sans-serif*, mais apropriada para o consumo digital e formatar todo o texto em estilo normal com a seguinte exceção: comunicações mediúnicas e trechos bíblicos serão em *itálico* e trechos originalmente realçados em _itálico_ serão mudados para **negrito**.

Usaremos o _blockquote_ para identificar visualmente as comunicações mediúnicas. Destacaremos trechos bíblicos usando o mesmo método e atribuindo o livro, capítulo, e versículo, assim realçando a concordância entre as duas obras.

Adicionalmente, numerais romanos foram substituídos por seus equivalentes arábicos (exceção para títulos, tais como São Luís, IX da França, e séculos).

### Formatação de texto (arquivo MD)

Exemplificado abaixo estão exemplos da formatação que escolhemos.

#### Questões (arquivo MD)

---

`LDE.q3` #️⃣ 3. Poder-se-ia dizer que **Deus** é o infinito?

>Definição incompleta. Pobreza da linguagem humana, **insuficiente** para definir o que está acima da linguagem dos homens.

Deus é infinito em suas perfeições, mas o infinito é uma abstração. Dizer que Deus é o infinito é tomar o atributo de uma coisa pela coisa mesma, é definir uma coisa que não está conhecida por uma outra que não o está mais do que a primeira. 

---

#### Trechos bíblicos (arquivo MD)

---

E disse Jesus:

>A cada um, de acordo com suas obras.
>
>✝️ Romanos, cap. 2, vers. 6

---
