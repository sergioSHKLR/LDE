# 👻 O Livro dos Espíritos

1️⃣ Primeiro sub *repo* de [doutrina.org](https://github.com/sergioSHKLR/doutrina.org), *hosted* no Github.

## 1. Direto ao ponto                       

- 📔 [LDE-2023-07-13.md](./releases/LDE-2023-07-13.md)

## 2. Objetivo

Intencionamos criar versões mais dinâmicas das cinco obras básicas, listadas abaixo.

1. O Livro dos Espíritos
2. O Livro dos Médiuns
3. O Evangelho segundo o Espiritismo
4. O Céu e o Inferno
5. A Gênese

Utilizaremos de emojis, cores, tipografia, padrões de formato, e um código mestre que possa ser usado para localizar e correlacionar diferentes partes destas mesmas obras. Adicionaremos *links* internos quando a indicação para uma leitura adicional é feita (por exemplo, Veja-se questão X de O Livro Y).

Em uma fase posterior, iremos adicionar links externos para artigos, mapas, ilustrações, e definições de termos pouco usados.

## 3. Análise

Gostaríamos que nossa versão não sofresse da rigidez do PDF (páginas de tamanho fixo), fosse de mais fácil uso que um eBook (sem necessidade de um aplicativo especial), e não usasse *DRM* (como AZW do *Kindle*). Formatos de processadores de texto (como DOC, DOCX, ou ODF) foram rejeitados por não serem capazes de lidar com arquivos deste comprimento. Formatos livres e simples como TXT ou RTF são muito pobres em formatação de texto e não permitem a fidelidade desejada.

## 4. Formato de arquivo

Decidimos então por adotar o formato *MarkDown* (.md) pela sua fácil edição e capacidade de formatação de texto. Entretanto, por necessidade, tivemos que utilizar várias *tags* HTML, tornando o arquivo em um híbrido MD&HTML. Para satisfazer a necessidade de programadores que visam utilizar nossos arquivos para criar outros, mantivemos uma versão MD pura no branch `coding`.

## 5. Obra original

Optamos por utilizar a coletânea traduzida do original francês de Allan Kardec para o português de Brasil por Guillon Ribeiro e Manuel Quintão, e impressa pela Federação Espírita Brasileira (Copyright 1944). Agradecemos a Federação Espírita Brasileira (FEB), por disponibilizar gratuitamente o PDF das obras básicas, todas [nesta](https://www.febnet.org.br/portal/2022/08/10/obras-de-allan-kardec-3/) página (verificada em 02 de maio de 2023).

### 5.1. Formatação de texto (livro impresso)

Como exemplificado abaixo (trecho intencionalmente modificado do original), a editora usou a divisão visual (linhas em branco; aspas) e estilística (fonte normal; itálico; fonte menor) para separar elementos (origem humana; origem espiritual) e denotar realce ou grifo. 

#### 5.1.1. Questões (livro impresso)

Como se vê, na pergunta, a palavra **Deus** foi realçada em estilo normal, visto que a sentença se encontra em estilo itálico. Já na resposta, palavra **insuficiente** foi realçada em estilo itálico, visto que a sentença se encontra em estilo normal. De modo a diferenciar os comentários de Kardec das mensagens de Espíritos, usou-se uma fonte ligeiramente menor em tamanho.

---

<span style="font-family: serif;">
<b>3.</b><span style="font-style: italic; margin-left: 30px;">Poder-se-ia dizer que <span style="font-style: normal">Deus</span> é o infinito?</span></span><br />

<p style="font-family: serif; margin-left: 40px;">“Definição incompleta. Pobreza da linguagem humana, <i>insuficiente</i> para definir o que está acima da linguagem dos homens.”</p>

<span style="font-family: serif; margin-left: 70px; font-size: 90%;">Deus é infinito em suas perfeições, mas o infinito é uma abstração. Dizer que Deus é o <i>infinito</i> é tomar o atributo de uma coisa pela coisa mesma, é definir uma coisa que não está conhecida por uma outra que não o está mais do que a primeira.</span></span>

---

#### 5.1.2 Trechos bíblicos

Trechos bíblicos, em geral, não foram separados ou atribuídos por livro, capítulo e versículo.

---

<span style="font-family: serif;">E disse Jesus: “A cada um, de acordo com suas obras.”
</span>

--- 

Consideramos estas escolhas de formatações demasiada sutis (não chamam a atenção do leitor com eficiência), além de introduzir dificuldades na padronização programática. Adicionalmente, as mesmas não são apropriadas para a análise e formatação automática por meio de *scripts*, sendo o método que nosso maior colaborador, **<a href="https://github.com/JhonnyBn">JhonnyBn</a>**, criou para automatizar parte de nosso processo.

## 6. Método

Em primeiro lugar, teríamos que estabelecer padrões de divisão, hierarquia, e formatação de texto que mantivessem a fidelidade ao original, não em forma, mas em conteúdo.

Analisando a divisão do livro em partes, decidimos criar uma seção anterior à `LDE-1` 🗂️ Parte 1 como `LDE-0` 🗂️ Parte 0, e dar-lhe o título de Pré-textual. Similarmente, criamos uma seção posterior à `LDE-5` 🗂️ Parte 5, e por dar-lhes o nome de `LDE-6` 🗂️ Parte 6 e o título de Pós-textual.

## 7. Padronização

Decidimos utilizar um tipo *sans-serif*, mais apropriada para o consumo digital e formatar todo o texto em estilo normal com a seguinte exceção: comunicações mediúnicas e trechos bíblicos serão em *itálico* e trechos originalmente realçados em _itálico_ serão mudados para **negrito**.

Usaremos o _blockquote_ para identificar visualmente as comunicações mediúnicas. Destacaremos trechos bíblicos usando o mesmo método e atribuindo o livro, capítulo, e versículo, assim realçando a concordância entre as duas obras.

Adicionalmente, numerais romanos foram substituídos por seus equivalentes arábicos (exceção para títulos, tais como São Luís, IX da França, e séculos).

### 7.1. Formatação de texto (arquivo MD)

Exemplificado abaixo estão exemplos da formatação que escolhemos.

#### 7.1.1 Questões (arquivo MD)

---

`LDE.q3` #️⃣ 3. Poder-se-ia dizer que **Deus** é o infinito?

>Definição incompleta. Pobreza da linguagem humana, **insuficiente** para definir o que está acima da linguagem dos homens.

Deus é infinito em suas perfeições, mas o infinito é uma abstração. Dizer que Deus é o infinito é tomar o atributo de uma coisa pela coisa mesma, é definir uma coisa que não está conhecida por uma outra que não o está mais do que a primeira. 

---

#### 7.1.2 Trechos bíblicos (arquivo MD)

---

E disse Jesus:

>A cada um, de acordo com suas obras.
>
>✝️ Romanos, cap. 2, vers. 6

---

### 7.2. Legenda

Individualmente, iremos identificar os livros pelos emojis e/ou siglas abaixo.

| **Emoji** | **Sigla** | **Livro** |
|---|---|---|
| 👻 | `LDE` | O Livro dos Espíritos |
| ✒️ | `LDM` | O Livro dos Médiuns |
| 🕊️ | `ESE` | O Evangelho segundo o Espiritismo |
| 🔥 | `CEU` | O Céu e o Inferno |
| 🌱 | `GEN` | A Gênese |

Dentro deste livro, usaremos os emojis abaixo para identificar elementos individuais ou grupamentos dos mesmos. Note também o correspondente código mestre.

| **Emoji** | **Descrição** | **Conteúdo** | **Código chave** |
|---|---|---|---|
| 📔 | livro | obra completa | `LDE` |
| 🗂️ | parte | subdivisão da obra | `LDE-X` |
| 📑 | capítulo | subdivisão de partes | `LDE-X-XX` |
| 📃 | seção | subdivisão de capítulos | `LDE-X-XX-XX` |
| #️⃣ | questão | pergunta, reposta e comentário * | `LDE.qX` |

/* Existem exceções deste formato, tais como 59, 100-113, 222, 257, 455 e 872.

##### 7.2.1. Adicionais

| **Emoji** | **Descrição** | **Conteúdo** |
|---|---|---|
| :latin_cross: | trecho bíblico | trecho atribuído com livro, capítulo e versículo |
| :point_right: | segmento relacionado | indicação para leitura complementar |

<!--
| 🗃️ | Índice Geral | coleção de 🏷️ _tags_ |
| 🏷️ | _tag_ | agrupa #️⃣ questões e/ou 📃 seções por assunto |
| ⚜️ | fim | término de um elemento | 
-->

### 6.3. Hierarquia 

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

### 6.4. Código chave

Para facilitar a organização hierárquica, localização, correlação de items, e brevidade, um código chave foi criado. Para isso, pequenas mudanças foram feitas ─ em forma, não em conteúdo. Este código alfanúmerico é demonstrado abaixo.

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

## 8. Navegação

De modo a evitar um sumário extremamente longo, decidimos por dividi-lo em partes incrementais. Ao começo do livro temos o sumário das partes e ao começo dos capítulos temos o sumário de seções. Ao término de cada segmento, você encontra este emoji 🔼, que ao ser clicado, lhe retorna ao nível imediatamente superior (por exemplo, de seção para capítulo ou de capítulo para parte).

## 9. Controle de Qualidade

Tentamos ao máximo manter a integralidade e fidelidade da obra, entretanto, no curso de adaptação do conteúdo para o consumo móvel (*tablets* e celulares) e por claridade/brevidade se achou mais apropriado a mudança do título de alguns capítulos ou sua ordem de apresentação, de modo a obedecer a um padrão de conjunto. Extremo cuidado foi tomado para que somente a forma fosse alterada, e em nenhum modo, o conteúdo do mesmo.

Em caso de erros, por favor, entrem em contato conosco para assegurar que a devida correção seja feita.

## 10. Autor

Sou um Americano nato, criado no Brasil desde 1976, e em 1997 resolvi retornar aos EUA aonde me alistei e servi na Marinha por quase 21 anos. Aposentado desde 2018, veterano das guerras do Iraque e Afeganistão (4 estrelas de campanha), sou auto-didata em programação *front-end* (HTML e CSS). Venho estudando a Doutrina Espírita desde 2013, por ocasião do casamento com minha esposa Mai, quem inspirou este projeto e muitos outros. Estes mesmos, disponíveis em [SHKLR.org](https://shklr.org) almejam a disseminação da Filosofia e Ciência Espírita tal como codificada por Allan Kardec.

## 11. Agradecimentos

À Deus, e aos três anjos que colocou ao meu lado. O da guarda, minha esposa, Mai, e nossa gatinha, Nina. Aos grupos espíritas de Tampa, Jacksonville, e Palm Beach, na Flórida, e o de Washington D.C, todos nos EUA. Também à Brian Foster (*in memoriam*) e ao meu amigo e mentor, Manoel Seabra, um dos fundadores do Love and Wisdom, de Largo, Flórida, EUA. Em especial, à João Neto, de Uberlândia, Minas Gerais, Brasil, programador e quem nos economizou meses de fastidiosa digitação e revisão. Adicionalmente, ele criou *scripts* que possibilitam a conversão (duplex) do formato MD para vários outros.

Deus abençoa, sempre!

![Sergio SHKLR](/images/sign.png)

| cargo | organização | website | email |
| --- | --- | --- | --- |
| 🎩 Fundador | ⭕ SHKLR | 🌐 [shklr.org](https://shklr.org) | 💌 [doutrina@shklr.org](mailto:doutrina@shklr.org?subject=LDE.md) |

## 12. Notas

- **LDE-YYYY-MM-DD.md** e seus variantes são licenciados sob [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.pt_BR). A licença aplica-se somente ao formato (diagramação, uso de emojis, tipografia, hierarquia, código mestre, etc) e NÃO ao conteúdo. Nosso código-fonte é disponível em https://github.com/sergioSHKLR/1lde.

- Nossos projetos não tem fins lucrativos ou de subsistência. Absolutamente nenhum ganho, compensação, troca, benefício, ou doação é solicitada, oferecida, feita, aceita, ou sub-entendida.

- Não exercemos direitos sobre as obras originais, suas traduções, ou derivativos que pertencem aos seus respectivos proprietários e/ou herdeiros.

- O nome e/ou logotipo de instituições, grupos, organizações, ou sociedades não constituem aprovação ou endosso. Ademais, estas entidades não são responsáveis pela qualidade de nossos serviços e/ou produtos.

- Uma ofensa aos direitos autorais não se constitui desde que se limite o uso de acordo com o [Artigo 46, Capítulo IV, Lei Nº 9.610, de 19 de Fevereiro de 1998](http://www.planalto.gov.br/ccivil_03/leis/l9610.htm#:~:text=Art.%2046.%20N%C3%A3o%20constitui%20ofensa%20aos%20direitos%20autorais%3A). Reproduzimos abaixo alguns trechos pertinentes.

 - Título II, Capítulo I, Art. 7º, § 3º – No domínio das ciências, a proteção recairá sobre a forma literária ou artística, não abrangendo o seu conteúdo científico ou técnico, sem prejuízo dos direitos que protegem os demais campos da propriedade imaterial.

    - Título III, Capítulo IV, Art. 46 – Não constitui ofensa aos direitos autorais:

       - I – a reprodução
       - III – a citação em livros, jornais, revistas ou qualquer outro meio de comunicação, de passagens de qualquer obra, para fins de estudo, crítica ou polêmica, na medida justificada para o fim a atingir, indicando-se o nome do autor e a origem da obra.

- Como a formatação final de um arquivo MD depende da plataforma de visualização utilizada, não podemos garantir que seu resultado não contenha desvios do padrão GitHub. O mesmo ocorre com a visualização de emojis, que podem sofrer de desvios de formato em virtude da plataforma aonde o conteúdo é acessado.

