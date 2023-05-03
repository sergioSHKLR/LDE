# Um dos cinco repositórios de Doutrina.org

## Direto ao ponto                                              

O Livro dos Espíritos (ISBN 978-85-7328-728-8) digitalizado (manualmente, de parágrafo em parágrafo) em duas opções:

- um único arquivo                                             |
- ~~separado em 253 partes~~ (*defasadas em virtude de mudanças recentes no arquivo único, que é a fonte das partes. Voltarão a ser disponíveis quando o RELEASE ficar pronto*)

---

## Apresentação

Nosso projeto almeja a disseminação da Filosofia e Ciência Espírita tal como codificada por Allan Kardec, traduzida do orginal francês para o português por Guillon Ribeiro e Manuel Quintão, e impressa pela [Federação Espírita Brasileira](https://www.febnet.org.br). Agradecemos a FEB, por disponibilizar gratuitamente o PDF das obras básicas, todas disponíveis [nesta](https://www.febnet.org.br/portal/2022/08/10/obras-de-allan-kardec-3/) página (verificada em 02 de maio de 2023).

O objetivo seria de criar um arquivo que não sofresse da rigidez do PDF (páginas de tamanho fixo), fosse de mais fácil edição que um ePUB, e não usasse DRM (como AZW do Kindle). Formatos proprietários como DOC ou DOCX foram rejeitados. Formatos livre e simples como TXT ou RTF não são capazes de usar imagens ou tabelas. Formatos como ODF não conseguem suportar arquivos de tal comprimento com eficiência. 

Decidi então por adotar o formato MarkDown (.md) pela sua fácil edição. Adicionalmente, o formato permite que o mesmo sirva de fonte para conversões em arquivos diversos, tal como HTML/CSS (em SSG), JSON, etc. Isto ainda facilita a utilização por programadores que queiram usar o mesmo para servir de base ou banco de dados para seus próprios projetos, tais como *apps*.

##  Análise

Em primeiro lugar, teríamos que estabelecer padrões de formatação que mantivessem a fidelidade ao original, não em forma, mas em conteúdo.

Analisando a particionamento do livro em partes, decidi nomear a seção anterior à *Parte 1* como *Parte 0*, e dar o título de *Pré-textual*. Considerando as seções que seguem a `lde.5` *Parte 5 - Conclusão*, decidimos por dar-lhes o nome de *Parte 6* e o título de *Pós-textual*.


A formatação original da Editora, na  qual perguntas se encontravam em itálico e repostas em fonte normal forçou que trechos em realce se fizessem na fonte oposta, como no exemplo abaixo:

---

| Formatação original do livro impresso |
| ------------------------------------- |

X. *Pergunta lorem ipsum dolor sit* amet, consectetur adipiscing elit?

Resposta sed do eiusmod *tempor* incididunt ut labore et dolore magna aliqua.

Comentário de Kardec Duis aute irure dolor in reprehenderit in voluptate.

---

Obs. Na Pergunta, palavra 'amet' foi realçada em fonte normal, visto que a sentença se encontra em itálico. Na Resposta, palavra 'tempor' foi realçada em itálico, visto que a sentença se encontra em fonte normal.

Outra forma originalmente utilizada para diferenciar os comentários de Kardec das mensagens de Espíritos, foi o de usar uma fonte ligeiramente menor em tamanho. Considero estas escolhas de formatações demasiada sutis (não chamam a atenção do leitor com eficiência), além de introduzir confusão na padronização. Adicionalmente, as mesmas não são apropriada para o formato *Markdown*, ou a análise e formatação automática por meio de *scripts*, sendo o método que nosso maior colaborador, **<a href="https://github.com/JhonnyBn">JhonnyBn</a>**, criou para automatizar o processo.

Outra pequenas mudança foi a substituição de quase todos os numerais romanos por seus equivalentes arábicos. 

## Solução

Sendo assim, decidi formatar todo o texto em fonte normal com as seguintes exceções: Os trechos originalmente em *itálico* foram mudados para **negrito**; respostas dos Espíritos (entre aspas) e quotações bíblicas serão destacadas em *blockquote*, e identificadas com livro, capítulo e versículo. Comentários de Kardec viraram *nested blockquotes* como no exemplo abaixo.

---

| Formatação de Doutrina.org |
| -------------------------- |

 X. Pergunta lorem ipsum dolor sit **amet**, consectetur adipiscing elit? 

 > Resposta sed do eiusmod **tempor** incididunt ut labore et dolore magna aliqua.
 >
 > > Comentário de Kardec Duis aute irure dolor in reprehenderit in voluptate.

E disse Jesus: 

>"A cada um, de acordo com suas obras." Romanos, cap. 2, vers. 6

---

Acredito que o formato acima utiliza com muita mais eficiência o realce de certos trechos. Ademais, comentários de Kardec são visualmente ligados à resposta à que se referem.

Para facilitar a organização hierárquica, localização, correlação de items, e brevidade, um código mestre foi criado. Para isso, pequenas mudanças foram feitas -- em forma, não em conteúdo. Este código alfanúmerico é demonstrado abaixo.

### Estrutura de hieraquia

<pre>
📔 Livro
 |
 └── 🗂️ Parte
     |
     └── 📑 Capítulo
         |
         └── 📄 Item
</pre>

### Código alfanúmerico

<pre>
📄 lde.0.00.00
    │  │  │  │
    │  |  |  └── 📄 Item
    |  |  |
    │  |  └── 📑 Capítulo
    |  |
    │  └── 🗂️ Parte
    |
    └── 📔 Livro
</pre>

juntamente com

<pre>
📄 lde.q X a
    │  │ │ │
    │  | | └── Sub-item
    |  | |
    │  | └── Número
    |  |
    │  └── Questão
    |
    └── 📔 Livro
</pre>

Como ilustrado acima, usamos três letras para o livro, e de um a dois dígitos para partes, capítulos, e itens. Em especial, no LDE, usamos a letra `q`, de um a quatro dígitos, e uma letra minúscula para sub-itens de modo a designar uma pergunta específica (ex. `lde.q909a`).

Tentamos ao máximo manter a integralidade e fidelidade da obra, entretanto, no curso de adaptação do conteúdo para o consumo móvel (**tablets** e celulares) e por claridade/brevidade se achou mais apropriado a mudança do título de alguns capítulos ou sua ordem de apresentação, de modo a obedecer a um padrão de conjunto. Extremo cuidado foi tomado para que somente a forma fosse alterada, e em nenhum modo, o conteúdo do mesmo.

Em caso de erros, por favor, entrem em contato conosco para assegurar que a devida correção seja feita.

Deus abençoa, sempre!

![Sergio SHKLR](./assinado.png)

- ⭕ SHKLR.org
- Fundador

Clique abaixo para abrir o livro em arquivo único.

- [lde-single-file.md](./lde-single-file.md)



**Notas**

- **lde-single-file.md** é licenciado sob [CC BY-NC-SA 4.0](https://creativecommons.org/licenses/by-nc-sa/4.0/deed.pt_BR). A licença aplica-se somente ao formato (hierarquia, código mestre, diagramação, uso de ícones, e tipografia) e NÃO ao conteúdo. Nosso código-fonte é disponível em https://github.com/sergioSHKLR/1lde.

- Não exercemos direitos sobre a obra original, suas traduções, ou derivativos que pertencem aos seus respectivos proprietários ou herdeiros.

- Uma ofensa aos direitos autorais não se constitui desde que se limite o uso de acordo com o [Artigo 46, Capítulo IV, Lei Nº 9.610, de 19 de Fevereiro de 1998](http://www.planalto.gov.br/ccivil_03/leis/l9610.htm#:~:text=Art.%2046.%20N%C3%A3o%20constitui%20ofensa%20aos%20direitos%20autorais%3A). Reproduzimos abaixo alguns trechos pertinentes.

  - Título II, Capítulo I, Art. 7º, § 3º – No domínio das ciências, a proteção recairá sobre a forma literária ou artística, não abrangendo o seu conteúdo científico ou técnico, sem prejuízo dos direitos que protegem os demais campos da propriedade imaterial.

  - Título III, Capítulo IV, Art. 46 – Não constitui ofensa aos direitos autorais:
    - I – a reprodução
    - III – a citação em livros, jornais, revistas ou qualquer outro meio de comunicação, de passagens de qualquer obra, para fins de estudo, crítica ou polêmica, na medida justificada para o fim a atingir, indicando-se o nome do autor e a origem da obra.

- O nome ou logotipo de instituições, grupos, organizações, ou sociedades não constituem aprovação ou endosso. Ademais, estas entidades não são responsáveis pela qualidade de nossos serviços, produtos, ou informações.

- Nossos projetos não tem fins lucrativos. Absolutamente nenhum ganho, compensação, troca, benefício, ou doação é solicitada, oferecida, feita, aceita, ou sub-entendida.

- Como a formatação final de um arquivo MD depende da plataforma de visualização utilizada, não podemos garantir que seu resultado não contenha desvios do padrão GitHub. O mesmo ocorre com a visualização de Emojis, que podem sofrer de desvios de formato.
