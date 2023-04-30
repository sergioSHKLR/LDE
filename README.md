# Um dos cinco repositórios de Doutrina.org

O Livro dos Espíritos (ISBN 978-85-7328-728-8) digitalizado (manualmente, de parágrafo em parágrafo) em duas opções:

- um único arquivo.
- ~~separado em 253 partes (*defasadas em virtude de mudanças recentes no arquivo único, que é a fonte das partes*)~~

A formatação original da Editora, na  qual perguntas se encontravam em itálico e repostas em fonte normal forçou que trechos em realce se fizessem na fonte oposta, como no exemplo abaixo:

---
| Formatação original do livro impresso |
| --- |

X. *Pergunta lorem ipsum dolor sit* amet, consectetur adipiscing elit?

Resposta sed do eiusmod *tempor* incididunt ut labore et dolore magna aliqua.

Comentário de Kardec Duis aute irure dolor in reprehenderit in voluptate.

---

Obs. Na Pergunta, palavra 'amet' realçada em fonte normal, visto que a sentença se encontra em itálico. Na Resposta, palavra 'tempor' realçada em itálico, visto que a sentença se encontra em fonte normal.

Outra forma originalmente utilizada para diferenciar os comentários de Kardec das mensagens de Espíritos, foi o de usar uma fonte ligeiramente menor em tamanho. Considero estas escolhas de formatações demasiada sutis (não chamam a atenção do leitor com eficiência), além de introduzir confusão na padronização. Adicionalmente, as mesmas não são apropriada para o formato *Markdown*, ou a análise e formatação automática por meio de *scripts*, sendo o método que nosso maior colaborador, <a href="https://github.com/JhonnyBn">JhonnyBn</a>, criou para automatizar o processo.

Sendo assim, decidi formatar todo o texto em fonte normal com as seguintes exceções: Os trechos originalmente em *itálico* foram mudados para **negrito**. Trechos entre aspas (mensagens espirituais) viraram *blockquote*. Comentários de Kardec viraram *nested blockquotes* como no exemplo abaixo.

---

| Formatação de Doutrina.org |
| --- |

 X. Pergunta lorem ipsum dolor sit **amet**, consectetur adipiscing elit? 
 > Resposta sed do eiusmod **tempor** incididunt ut labore et dolore magna aliqua.
 >> Comentário de Kardec Duis aute irure dolor in reprehenderit in voluptate.

---

Para facilitar a organização hierárquica, localização, correlação de items, e brevidade, um código mestre foi criado. Para isso, pequenas mudanças foram feitas -- em forma, não em conteúdo. Este código alfanúmerico é demonstrado abaixo.

## Estrutura de hieraquia

<pre>
📔 Livro
 |
 └── 🗂️ Parte
     |
     └── 📑 Capítulo
         |
         └── 📄 Item
</pre>

> Livros podem ser:
> - `lde` (O Livro dos Espíritos)
> - `ldm` (O Livro dos Médiuns)
> - `ese` (O Evangelho segundo o Espiritismo)
> - `ceu` (O Céu e o Inferno)
> - `gen` (A Gênese)

## Código alfanúmerico

<pre>
📄 liv.0.00.00
    │  │  │  │
    │  |  |  └── 📄 Item
    |  |  |
    │  |  └── 📑 Capítulo
    |  |
    │  └── 🗂️ Parte
    |
    └── 📔 Livro
</pre>

Como ilustrado acima, usamos três letras para o livro, e de um a dois dígitos para partes, capítulos, e itens. Em especial, no LDE, usamos a letra `q`, de um a quatro dígitos, e uma letra minúscula para sub-itens de modo a designar uma pergunta específica (ex. `lde.q909a`).

Em sequência, converteremos os outros livros da codificação. Ao término de GEN, iremos criar um *fork* para incluir *inline links* (dicionário, Wikipédia, videos, etc), figuras, citações biblícas, e outros aperfeiçoamentos.

# Amai-vos e instruí-vos.

Clique abaixo para abrir o livro em arquivo único.

- [LDE](./lde-single-file.md)

<img src="./lde-capa.jpg" alt="capa de O Livro dos Espíritos" style="max-width: 50%">
