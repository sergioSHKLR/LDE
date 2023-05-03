| Formatação de **lde-single-file.md** |
| -------------------------- |

`lde.qX` #️⃣ X. Pergunta lorem ipsum dolor sit **amet**, consectetur adipiscing elit? 

 > Resposta sed do eiusmod **tempor** incididunt ut labore et dolore magna aliqua.
 >
 > > Comentário de Kardec Duis aute irure dolor in reprehenderit in voluptate.

E disse Jesus: 

>"A cada um, de acordo com suas obras." Romanos, cap. 2, vers. 6

---

Decidi formatar todo o texto em estilo normal com as seguintes exceções: Os trechos originalmente em *itálico* foram mudados para **negrito**; respostas dos Espíritos (entre aspas) e quotações bíblicas serão destacadas em *blockquote*, e identificadas com livro, capítulo e versículo. Comentários de Kardec viraram *nested blockquotes* como no exemplo acima.

Para facilitar a organização hierárquica, localização, correlação de items, e brevidade, um código mestre foi criado. Para isso, pequenas mudanças foram feitas -- em forma, não em conteúdo. Este código alfanúmerico é demonstrado abaixo.

### Estrutura

#### Legenda

Aonde os emojis abaixo denotam a seguinte arrumação, do menor ao maior conjunto:

<pre>
#️⃣ ─ (:question:) itens numerados, dentro do formato pergunta+resposta; código mestre `lde.qX`
📄 ─ (:page_facing_up:) assuntos, geralmente agrupados em 📑 capítulos mas podem existir diretamente 
      abaixo de partes 🗂️; código mestre `lde.X.X.X`
🟨 ─ (:yellow_square:) títulos de assuntos tratados; referem-se à #️⃣ itens ou #️⃣ perguntas; sem código
      mestre; reservado para uso no Indíce geral
📑 ─ (:bookmark_tabs:) capítulos, contendo um ou mais 📄 itens; código mestre `lde.X.X`
🗂️ ─ (:card_index_dividers:) partes, contendo um ou mais 📑 capítulos, podendo também ter 📄 itens 
      individuais; código mestre `lde.X`
📔 ─ (:notebook_with_decorative_cover:) a obra básica, contendo partes, capitulos e itens. Código mestre `lde`
⚜️ ─ (:fleur_de_lis:) fim de uma seção
</pre>

#### Hierarquia

<pre>
📔 livro
 |
 └── 🗂️ parte
     |
     └── 📑 capítulo
         |
         └── 📄 item
         └── #️⃣ pergunta numerada

🟨 ── assunto
</pre>

#### Código mestre

<pre>
lde.X.X.X
 │  │ │ │
 │  | | └── 📄 assunto
 |  | |
 │  | └── 📑 capítulo
 |  |
 │  └── 🗂️ parte
 |
 └── 📔 livro
</pre>

juntamente com

<pre>
#️⃣ lde.q X a
    │  │ │ │
    │  | | └── sub-pergunta
    |  | |
    │  | └── pergunta
    |  |
    │  └── questão
    |
    └── 📔 livro
</pre>
Como ilustrado acima, usamos três letras para o livro, e de um a dois dígitos para partes, capítulos, e itens. Em especial, no LDE, usamos a letra `q`, de um a quatro dígitos, e uma letra minúscula para sub-itens de modo a designar uma pergunta específica (ex. `lde.q909a`).

---

### Controle de Qualidade

Tentamos ao máximo manter a integralidade e fidelidade da obra, entretanto, no curso de adaptação do conteúdo para o consumo móvel (**tablets** e celulares) e por claridade/brevidade se achou mais apropriado a mudança do título de alguns capítulos ou sua ordem de apresentação, de modo a obedecer a um padrão de conjunto. Extremo cuidado foi tomado para que somente a forma fosse alterada, e em nenhum modo, o conteúdo do mesmo.

Em caso de erros, por favor, entrem em contato conosco para assegurar que a devida correção seja feita.

### Agradecimentos

Em primeiro lugar, Deus, e aos três anjos que colocou ao meu lado. O da guarda, minha esposa, Mai, e nossa gatinha, Nina. Aos grupos espíritas de Tampa, Jacksonville, Washington D.C, e Palm Beach. Também a Brian Foster (in memoriam) e ao meu amigo e mentor, Manoel Seabra, um dos fundadores do Love and Wisdom SS, de Largo, FL, EUA. João Neto, de Uberlândia, MG, Brasil, programador e quem nos economizou meses em digitação e revisão.

Deus abençoa, sempre!

![Sergio SHKLR](./assinatura.png)

🪨 Fundador | ⭕ SHKLR.org | 🌐 [shklr.org](https://shklr.org) | 📞 [+1 (281) 406-0950](tel:+12814060950) (WhatsApp)

---
