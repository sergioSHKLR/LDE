# O LIVRO DOS ESPÍRITOS
Uma das cinco Obras Básicas da Ciência e Filosofia Espírita.

## 0. Direto ao ponto                                              

O Livro dos Espíritos (ISBN 978-85-7328-728-8), digitalizado e em duas opções:

- um único arquivo
- ~~separado em 253 partes~~ (*defasadas em virtude de mudanças recentes no arquivo único, que é a fonte das partes. Voltarão a ser disponíveis quando o RELEASE ficar pronto*)

## 1. Objetivo

Intencionamos criar versões mais dinâmicas das Obras Básicas, utilizando emojis, cores, tipografia, padrões de formato, e criando um código mestre que possa ser usado para localizar e correlacionar diferentes partes destas mesmas obras.

## 2. Análise

Gostaríamos que nossa versão não sofresse da rigidez do PDF (páginas de tamanho fixo), fosse de mais fácil uso quem um eBook (sem necessidade de um aplicativo especial), e não usasse *DRM* (como AZW do *Kindle*). Formatos de processadores de texto (como DOC, DOCX, ou ODF) foram rejeitados por não serem capazes de lidar com arquivos deste comprimento. Formatos livres e simples como TXT ou RTF são muito pobres em formatação de texto e não permitem a fidelidade desejada.

## 3. Formato de arquivo

Decidimos então por adotar o formato *MarkDown* (.md) pela sua fácil edição e grande capacidade de formatação de texto. Adicionalmente, o formato permite que o mesmo sirva de fonte para conversões em arquivos diversos, tal como HTML & CSS (em SSG), JSON, etc. Isto ainda facilita a utilização por programadores que queiram usar o mesmo para servir de base ou banco de dados para seus próprios projetos, tais como *apps*.

## 4. Obra original

Decidimos utilizar a coletânea traduzida do original francês para o português por Guillon Ribeiro e Manuel Quintão, e impressa pela Federação Espírita Brasileira. Agradecemos a FEB, por disponibilizar gratuitamente o PDF das obras básicas, todas disponíveis [nesta](https://www.febnet.org.br/portal/2022/08/10/obras-de-allan-kardec-3/) página (verificada em 02 de maio de 2023).

### 4.1 Formatação de texto (livro impresso)

Originalmente usou-se a divisão visual (linhas em branco; aspas) e estilística (fonte normal; itálico; fonte menor) para separar elementos (origem humana; origem espiritual) e denotar realce ou grifo, como no exemplo abaixo (modificado do original para ilustração). Trechos bíblicos, em geral, não são separados ou atribuídos com livro, capítulo e versículo.

---

3. *Poder-se-ia dizer que* Deus *é o infinito?*

“Definição incompleta. Pobreza da linguagem humana, *insuficiente* para definir o que está acima da linguagem dos homens.”

Deus é infinito em suas perfeições, mas o infinito é uma abstração. Dizer que Deus é o infinito é tomar o atributo de uma coisa pela coisa mesma, é definir uma coisa que não está conhecida por uma outra que não o está mais do que a primeira.

---

Como se vê, na pergunta, a palavra 'Deus' foi realçada em estilo normal, visto que a sentença se encontra em estilo itálico. Já na resposta, palavra 'insuficiente' foi realçada em estilo itálico, visto que a sentença se encontra em estilo normal. De modo a diferenciar os comentários de Kardec das mensagens de Espíritos, usou-se uma fonte ligeiramente menor em tamanho. 

Consideramos estas escolhas de formatações demasiada sutis (não chamam a atenção do leitor com eficiência), além de introduzir confusão na padronização programática. Adicionalmente, as mesmas não são apropriadas para o formato *Markdown*, ou a análise e formatação automática por meio de *scripts*, sendo o método que nosso maior colaborador, **<a href="https://github.com/JhonnyBn">JhonnyBn</a>**, criou para automatizar o processo.

## 5. Método

Em primeiro lugar, teríamos que estabelecer padrões de formatação de texto que mantivessem a fidelidade ao original, não em forma, mas em conteúdo.

Analisando a divisão do livro em partes, decidimos nomear a seção anterior à *Parte 1* como *Parte 0*, e dar o título de *Pré-textual*. Considerando as seções que seguem a `lde.5` *Parte 5 - Conclusão*, decidimos por dar-lhes o nome de *Parte 6* e o título de *Pós-textual*. Inéditamente, iremos manter o Indíce Geral por admirar o extenso trabalho de criá-lo e sua valiosa função.

## 6. Padronização

Decidimos formatar todo o texto em estilo normal com as seguintes exceções: Os trechos originalmente em *itálico* foram mudados para **negrito**; respostas dos Espíritos (entre aspas) e trechos bíblicos serão destacadas em *blockquote* (linha cinza vertical, simples), e identificadas com livro, capítulo e versículo. Comentários de Kardec viraram *nested blockquotes* (linha cinza vertical, dupla). 

Considero que estas escolhas fazem um bom uso de elementos mais apropriados para o consumo digital (cores, tipografia sans-serif, icones, código hierárquico, etc). Adicionalmente, numerais romanos foram substituídos por seus equivalentes arábicos (exceção para títulos, tais como São Luís, IX da França).

### 6.1. Formatação de texto (1lde-single-file.md)

`lde.q3` #️⃣ 3. Poder-se-ia dizer que **Deus** é o infinito?

>“Definição incompleta. Pobreza da linguagem humana, **insuficiente** para definir o que está acima da linguagem dos homens.”
>>Deus é infinito em suas perfeições, mas o infinito é uma abstração. Dizer que Deus é o infinito é tomar o atributo de uma coisa pela coisa mesma, é definir uma coisa que não está conhecida por uma outra que não o está mais do que a primeira. ⚜️

E disse Jesus: 

>"A cada um, de acordo com suas obras." ✝️ Romanos, cap. 2, vers. 6

---

### 6.2. Legenda

Os emojis abaixo denotam a seguinte arrumação, do menor ao maior elemento ou grupamento.

| **Icone** | **Descrição** | **Conteúdo** | **Consiste de** | **Parte de** | **Código mestre** | **GFM** |
|---|---|---|---|---|---|---|
| #️⃣ | questão | pergunta+resposta (comentário) * | - | 📄 seções | `lde.qX` | question |
| 📄 | seção | subdivisão de capítulos | #️⃣ questões | 📑 capítulos | `lde.X.X.X` | page_facing_up |
| 📑 | capítulo | subdivisão de partes | 📄 seções | 🗂️ partes | `lde.X.X` | bookmark_tabs |
| 🗂️ | parte | subdivisão da obra | 📑 capítulos | 📔 livro | `lde.X` | card_index_dividers |
| 📔 | livro | obra completa | 🗂️ partes | 📚 Obras Básicas | `lde` | notebook_with_decorative_cover |

* Existem várias exceções como 59, 100-113, 222, 257, 455 e 872.

##### 6.2.1. Adicionais

| **Icone** | **Descrição** | **Conteúdo** | **GFM** |
|---|---|---|---|
| ✝️ | trecho bíblico | trecho, livro, capítulo, versículo | latin_cross |
| 🟨 | assunto | agrupa #️⃣ questões e/ou 📄 seções | yellow_square |
| ⚜️ | fim | parte final de um elemento | fleur_de_lis |

### 6.3. Hierarquia 

<pre>
📔 livro
 |
 └── 🗂️ parte
     |
     └── 📑 capítulo
         |
         └── 📄 seção
             |         
             └── #️⃣ questão

🟨 ── assunto
✝️ ── trecho bíblico
</pre>

### 6.4. Código mestre

Para facilitar a organização hierárquica, localização, correlação de items, e brevidade, um código mestre foi criado. Para isso, pequenas mudanças foram feitas -- em forma, não em conteúdo. Este código alfanúmerico é demonstrado abaixo.

<pre>
lde.X.X.X
 │  │ │ │
 │  | | └── 📄 seção
 |  | |
 │  | └── 📑 capítulo
 |  |
 │  └── 🗂️ parte
 |
 └── 📔 livro
</pre>

E em especial no LDE, o código para questões é modificado para:

<pre>
#️⃣ lde.q X a
    │  │ │ │
    │  | | └── sub-questão
    |  | |
    │  | └── número
    |  |
    │  └── questão 
    |
    └── 📔 livro
</pre>

Como ilustrado acima, usamos três letras para o livro, e de um a dois dígitos para partes, capítulos, e itens. Em especial, no LDE, usamos a letra `q`, de um a quatro dígitos, e uma letra minúscula para sub-itens de modo a designar uma pergunta específica (ex. `lde.q909a`).

## 7. Controle de Qualidade

Tentamos ao máximo manter a integralidade e fidelidade da obra, entretanto, no curso de adaptação do conteúdo para o consumo móvel (**tablets** e celulares) e por claridade/brevidade se achou mais apropriado a mudança do título de alguns capítulos ou sua ordem de apresentação, de modo a obedecer a um padrão de conjunto. Extremo cuidado foi tomado para que somente a forma fosse alterada, e em nenhum modo, o conteúdo do mesmo.

Em caso de erros, por favor, entrem em contato conosco para assegurar que a devida correção seja feita.

## 8. Autor

Sou um Americano nato, criado no Brasil desde 1976, e em 1997 resolvi retornar aos EUA aonde me alistei e servi na Marinha por quase 21 anos. Aposentado desde 2018, veterano das guerras do Iraque e Afeganistão (4 estrelas de campanha), sou auto-didata em programação *front-end* (HTML e CSS). Venho estudando a Doutrina Espírita desde 2013, por ocasião do casamento com minha esposa Mai, quem inspirou este projeto e muitos outros. Estes mesmos, disponíveis em [SHKLR.org](https://shklr.org) almejam a disseminação da Filosofia e Ciência Espírita tal como codificada por Allan Kardec. 

## 9. Agradecimentos

À Deus, e aos três anjos que colocou ao meu lado. O da guarda, minha esposa, Mai, e nossa gatinha, Nina. Aos grupos espíritas de Tampa, Jacksonville, e Palm Beach, Flórida, e o de Washington D.C, todos nos EUA. Também à Brian Foster (in memoriam) e ao meu amigo e mentor, Manoel Seabra, um dos fundadores do Love and Wisdom SS, de Largo, Flórida, EUA. Em especial, à João Neto, de Uberlândia, Minas Gerais, Brasil, programador e quem nos economizou meses de fastidiosa digitação e revisão.

Deus abençoa, sempre!

![Sergio SHKLR](./assinatura.png)

🪨 Fundador | ⭕ SHKLR.org | 🌐 [shklr.org](https://shklr.org) | 💬 [WhatsApp](https://wa.me/12814060950) | 📞 [+1 (281) 406-0950](tel:+12814060950)

## 10. Notas

- **1lde-single-file.md** é licenciado sob [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.pt_BR). A licença aplica-se somente ao formato (hierarquia, código mestre, diagramação, uso de ícones, e tipografia) e NÃO ao conteúdo. Nosso código-fonte é disponível em https://github.com/sergioSHKLR/1lde.

- Não exercemos direitos sobre as obras originais, suas traduções, ou derivativos que pertencem aos seus respectivos proprietários ou herdeiros.

- Uma ofensa aos direitos autorais não se constitui desde que se limite o uso de acordo com o [Artigo 46, Capítulo IV, Lei Nº 9.610, de 19 de Fevereiro de 1998](http://www.planalto.gov.br/ccivil_03/leis/l9610.htm#:~:text=Art.%2046.%20N%C3%A3o%20constitui%20ofensa%20aos%20direitos%20autorais%3A). Reproduzimos abaixo alguns trechos pertinentes.

  - Título II, Capítulo I, Art. 7º, § 3º – No domínio das ciências, a proteção recairá sobre a forma literária ou artística, não abrangendo o seu conteúdo científico ou técnico, sem prejuízo dos direitos que protegem os demais campos da propriedade imaterial.

  - Título III, Capítulo IV, Art. 46 – Não constitui ofensa aos direitos autorais:
    - I – a reprodução
    - III – a citação em livros, jornais, revistas ou qualquer outro meio de comunicação, de passagens de qualquer obra, para fins de estudo, crítica ou polêmica, na medida justificada para o fim a atingir, indicando-se o nome do autor e a origem da obra.

- O nome ou logotipo de instituições, grupos, organizações, ou sociedades não constituem aprovação ou endosso. Ademais, estas entidades não são responsáveis pela qualidade de nossos serviços, produtos, ou informações.

- Nossos projetos não tem fins lucrativos. Absolutamente nenhum ganho, compensação, troca, benefício, ou doação é solicitada, oferecida, feita, aceita, ou sub-entendida.

- Como a formatação final de um arquivo MD depende da plataforma de visualização utilizada, não podemos garantir que seu resultado não contenha desvios do padrão GitHub. O mesmo ocorre com a visualização de Emojis, que podem sofrer de desvios de formato.

---

## Versão Beta (em desenvolvimento)

Clique abaixo para abrir o livro em sua versão de arquivo único.

[1lde-single-file.md](./1lde-single-file.md)
