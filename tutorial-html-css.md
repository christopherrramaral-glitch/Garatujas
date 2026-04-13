# IA 26-webdesing.
## Introdução
 Está é uma diciplina introdutória as técnicas e práticas de **Web desing.**
 Focando nas linguagens de marcação (HTML), de estilo (CSS) e, brevemente, de programação (JavaScript). O objetivo é capacitar os alunos a criar e estilizar páginas web, abrindo caminho para o desenvolvimento de sites e aplicações web mais complexas no futuro.
### Antes do início
 É desejável que os alunos tenham um ambiente de desenvolvimento configurado em suas máquinas, incluindo um editor de código e um navegador web atualizado. Nesta disciplina, utilizaremos o Visual Studio Code como editor de código (por ser gratuito e o mais utilizado no mercado) e o Google Chrome como navegador web (pelos mesmos motivos).
- **HTML:** serve para **marcação**. Ou seja ele serve para dar estrutura para o conteudo de um site, normalmente é interpetrado visualmente. Contudo, o html é responsavel por organizar o conteudo de uma página para que qualquer tipo usuário. Portanto, a estrutura é fundamental para a acessibilidade de um site. 
- A estrutura HTML é composta por uma série de elementos, para definilos utilizamos uma ***tag*** (etiqueta) específica que compoẽm seu tipo de conteúdo e sua função. Por exemplo, `<h1>` é usado para títulos principais, `<p>` para parágrafos, `<a>` para links, entre outros. O HTML também permite a inclusão de atributos nas tags para fornecer informações adicionais sobre os elementos, como `class`, `id`, `src`, etc.
- Antes de seguirmos, imagine um editor de texto como o Microsoft Word ou o Google Docs. estes, você costuma selecionar um trecho de texto e aplicar uma formatação, como negrito, itálico ou sublinhado. No HTML para defenir isso usamos uma tag (etiqueta) para decidir a formatação desejada, sendo que a sintaxe do HTML é composta por tags (etiquetas) de abertura e fechamento, onde a etiqueta de abertura é escrita entre colchetes angulares `< >` e a etiqueta de fechamento é escrita da mesma forma, mas com uma barra `/` antes do nome da tag. Por exemplo, para criar um parágrafo em HTML, você usaria a tag `<p>` para abrir o parágrafo e `</p>` para fechá-lo. O conteúdo do parágrafo seria colocado entre essas duas tags.
- **O ( pinguim** de *geladeira* **)**/tudo em "()" ésta ipoteticamente vermelho/ comeu três iogurtes antes que a gravidade decidisse tirar férias na terça-feira.
Na animação acima, o usuário escreve em um editor a frase `O pinguim de geladeira comeu três iogurtes antes que a gravidade decidisse tirar férias na terça-feira.` e, então, executa algumas seleções de definição de formatação. A seguir, veremos, passo a passo, o equivalente em HTML para cada uma dessas seleções/formatações.

1. O usuário seleciona `O pinguim` e aplica a formatação de negrito.
  - Em HTML, o código correspondente seria `<strong>O pinguim</strong> de geladeira comeu três iogurtes antes que a gravidade decidisse tirar férias na terça-feira.`, onde a tag `<strong>` é usada para indicar que o texto deve ser exibido em negrito. No exemplo, a marcação começa com a tag `<strong>` e termina com a tag de fechamento `</strong>`, indicando que o texto entre essas tags deve ser exibido em negrito.
2. O usuário seleciona `geladeira` e aplica a formatação de itálico.
  - Em HTML, o código correspondente seria `<strong>O pinguim</strong> de <em>geladeira</em> comeu três iogurtes antes que a gravidade decidisse tirar férias na terça-feira.`, onde a tag `<em>` é usada para indicar que o texto deve ser exibido em itálico. No exemplo, a marcação começa com a tag `<em>` e termina com a tag de fechamento `</em>`, indicando que o texto entre essas tags deve ser exibido em itálico.
3. O usuário seleciona `pinguim de geladeira` e aplica a cor vermelha.
  - Em HTML, o código correspondente seria `<strong>O <span style="color: red;">pinguim de <em>geladeira</span></strong></em>`, onde a tag `<span>` é usada para aplicar estilos específicos a um trecho de texto, e o atributo `style` é usado para definir a cor do texto como vermelha. No exemplo, a marcação com a tag `<span>` começa antes de `O` e termina após `geladeira`, indicando que o texto entre essas tags deve ser exibido em vermelho.
> **⚠️ Nota:**
>
> O HTML é uma linguagem de marcação, e seu principal objetivo é estruturar o conteúdo de uma página web. Caso pesquise na internet, notará que existem outras tags para aplicar formatações como negrito e itálico, como `<b>` e `<i>`, respectivamente. No entanto, as tags `<strong>` e `<em>` são consideradas mais semânticas, pois indicam a importância do texto, enquanto as tags `<b>` e `<i>` são puramente de formatação visual. Portanto, é recomendado usar as tags semânticas para melhorar a acessibilidade e a compreensão do conteúdo.
>
> `<strong>` e `<em>` fazem sentido tanto para leitores sem deficiência quanto para leitores com deficiência, pois indicam a importância do texto, enquanto `<b>` e `<i>` são puramente de formatação visual e podem não ser interpretados corretamente por leitores de tela ou outros dispositivos assistivos.

Esta é a sintaxe básica do HTML, e existem muitas outras tags e atributos que podem ser usados para criar páginas web mais complexas e interativas. A sugestão de como aprender HTML é desenhar a estrutura de uma página web em um papel, identificando os diferentes elementos e suas relações, sempre se perguntando qual tag HTML seria mais adequada para representar cada elemento. Em seguida, você pode começar a escrever o código HTML correspondente, usando as tags apropriadas para estruturar o conteúdo da página. Lembre-se de que a prática é fundamental para aprender HTML, então experimente criar diferentes tipos de páginas web e explore as diversas tags e atributos disponíveis.

Ao final deste conteúdo, faremos um exercício prático para aplicar os conceitos aprendidos sobre HTML, onde você terá a oportunidade de criar uma página web simples, aplicando corretamente as tags HTML para estruturar o conteúdo de forma semântica e acessível. Este exercício ajudará a consolidar seu entendimento sobre a sintaxe do HTML e a importância de usar as tags apropriadas para cada tipo de conteúdo.

### Estrutura básica de um documento HTML

Outro ponto importante a ser abordado é a estrutura básica de um documento HTML. Todo documento HTML deve começar com a declaração do tipo de documento `<!DOCTYPE html>`, que informa ao navegador que o documento é um arquivo HTML5. Em seguida, o documento é estruturado em duas partes principais: o `<head>` e o `<body>`.

O `<head>` é a seção do documento onde são incluídas informações sobre a página, como o título, links para arquivos CSS, scripts JavaScript, meta tags (metainformações), entre outros. O conteúdo do `<head>` não é exibido diretamente na página, mas é essencial para o funcionamento e a aparência da página web.

O `<body>` é a seção do documento onde o conteúdo visível da página é colocado. É aqui que você adiciona os elementos HTML que compõem a estrutura e o conteúdo da página, como títulos, parágrafos, imagens, links etc. O conteúdo do `<body>` é o que os usuários veem quando acessam a página web.

A estrutura básica de um documento HTML pode ser representada da seguinte forma:

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
   <meta charset="UTF-8">
   <title>Título da Página</title>
   <!-- Links para arquivos CSS e scripts JavaScript podem ser adicionados aqui -->
</head>
<body>
   <!-- Conteúdo visível da página é adicionado aqui -->
</body>
</html>
```

## Aviso importante (simplificado)

Todo código HTML precisa ficar dentro da tag <html>, que é como a "caixa principal" da página. O atributo lang="pt-BR" diz que o conteúdo está em português do Brasil – isso ajuda programas de acessibilidade e o Google a entenderem o idioma. A linha <meta charset="UTF-8"> garante que letras com acento (como ç, ã, é) apareçam corretamente. A tag <title> define o título que aparece na aba do navegador e nos resultados de busca.

## Atributos HTML (simplificado)

Atributos HTML são informações extras que você coloca dentro de uma tag para dar mais detalhes sobre ela. Eles ficam dentro da tag de abertura e têm um nome e um valor, separados por =.

Exemplo:
- O atributo href é usado na tag <a> (link) para dizer para onde o link vai levar.
- O atributo src é usado na tag <img> (imagem) para indicar onde está o arquivo da imagem.

Exemplo prático:

Código:
<a href="https://www.google.com">Visite o Google</a>

Resultado explicado:
Aparece na tela um link clicável com o texto "Visite o Google". Quando o usuário clicar, será levado para o site do Google (que se abre no navegador).

## Lista completa de tags HTML

Se quiser ver todas as tags HTML existentes, você pode consultar:
- MDN Web Docs - Elementos HTML: https://developer.mozilla.org/pt-BR/docs/Web/HTML/Element
- W3Schools - HTML Tags: https://www.w3schools.com/TAGS/default.asp

## O que é CSS? (explicação para leigos)

CSS é a linguagem que enfeita a página web. Com ela você define:
- cores
- tamanhos de letra
- margens
- posicionamento de elementos

O legal é que o CSS fica separado do HTML. Assim:
- HTML = estrutura (o conteúdo)
- CSS = estilo (a aparência)

Isso deixa o código mais organizado e fácil de arrumar.

Exemplo passo a passo

Código HTML:

<!DOCTYPE html>
<html lang="pt-BR">
<head>
   <meta charset="UTF-8">
   <title>Exemplo de CSS</title>
   <link rel="stylesheet" href="styles.css">
</head>
<body>
   <h1>Olá, Mundo!</h1>
   <p>Este é um exemplo de CSS.</p>
</body>
</html>

A linha <link rel="stylesheet" href="styles.css"> puxa um arquivo separado chamado styles.css, que contém o seguinte código:

/* styles.css */
body {
  background-color: #f0f0f0;    /* fundo cinza bem clarinho */
  font-family: Arial, sans-serif; /* fonte mais legível */
}

h1 {
  color: #333333;               /* título em cinza escuro */
  text-align: center;           /* título centralizado */
}

p {
  color: #666666;               /* texto em cinza médio */
  font-size: 18px;              /* texto um pouco maior */
  margin: 20px;                 /* espaço em volta do texto */
}

Resultado visual (descrito em texto):
Uma página com fundo cinza bem clarinho. O título "Olá, Mundo!" aparece no meio da tela, em cinza escuro. O parágrafo aparece abaixo, em cinza médio, com letra maior e com uma margem de espaçamento em volta.

## O que acontece SEM o CSS?

Sem o CSS, o navegador usa um estilo padrão (chamado de user agent stylesheet). Esse estilo varia de navegador para navegador, mas geralmente é algo assim:

Fundo branco, letras pretas, sem margens especiais, sem cores diferentes, sem centralização. Tudo fica no canto esquerdo, parecendo um documento de bloco de notas.

Descrição da imagem "Sem CSS":
Você veria o título "Olá, Mundo!" em preto, no canto esquerdo, tamanho padrão, e o parágrafo embaixo também em preto, sem espaçamento especial. Nada de fundo cinza ou fonte Arial.

## Sintaxe do CSS (regras de escrita)

Cada regra de CSS tem esta estrutura:

seletor {
  propriedade: valor;
  propriedade: valor;
}

Explicação:
- seletor: diz em qual(is) elemento(s) aplicar o estilo (ex: h1, .titulo, #paragrafo1)
- propriedade: o que você quer mudar (ex: color, font-size)
- valor: como você quer mudar (ex: red, 16px)

Cada linha de propriedade: valor; termina com ponto e vírgula ;. O bloco todo é fechado com }.

## Seletores CSS (como "mirar" nos elementos)

Os seletores seguem a hierarquia do HTML (quem está dentro de quem). Por isso se chama "cascata" (Cascading Style Sheets).

Exemplo de HTML com hierarquia:

<main>
  <section>
    <p>Parágrafo dentro da seção</p>
  </section>
  <p>Parágrafo fora da seção</p>
</main>

Tipos de seletores mais comuns (tabela simplificada):

Tipo de seletor: Seletor de tipo (tag)
Exemplo: p { }
O que faz: Aplica estilo a todos os parágrafos

Tipo de seletor: Seletor de classe
Exemplo: .titulo { }
O que faz: Aplica a todos os elementos com class="titulo"

Tipo de seletor: Seletor de ID
Exemplo: #paragrafo1 { }
O que faz: Aplica a um único elemento com id="paragrafo1"

Tipo de seletor: Seletor de atributo
Exemplo: a[href="#"] { }
O que faz: Aplica a links cujo href seja "#"

Tipo de seletor: Pseudo-classe
Exemplo: p:first-child { }
O que faz: Aplica ao primeiro parágrafo dentro do pai

Seletores que usam hierarquia (descendentes, filhos, irmãos):

Tipo: Descendente
Exemplo: main section p { }
O que faz: Qualquer <p> dentro de <section> que está dentro de <main>

Tipo: Filho direto
Exemplo: main > section { }
O que faz: Apenas <section> que é filho direto de <main>

Tipo: Irmão adjacente
Exemplo: h1 + p { }
O que faz: O <p> que vem imediatamente depois de um `<h1>`

Tipo: Irmão generalizado
Exemplo: h1 ~ p { }
O que faz: Qualquer <p> que seja irmão de um `<h1>` (depois dele)

Exemplo visual (descrito em texto)

No código HTML mostrado acima, se usarmos o seletor main section p, apenas o parágrafo dentro da seção ficará verde. O parágrafo fora da seção não será afetado.

Descrição da imagem "Seletores CSS":
Imagine duas frases:
- "Parágrafo dentro da seção" -> escrito em verde.
- "Parágrafo fora da seção" -> continua com a cor padrão (preta). Isso mostra que o seletor só pegou o parágrafo que está dentro da hierarquia correta.

## Praticando HTML e CSS

Isso será tema da próxima aula.

See you space cowboy! 🚀
