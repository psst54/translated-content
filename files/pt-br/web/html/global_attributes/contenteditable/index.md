---
title: contenteditable
slug: Web/HTML/Global_attributes/contenteditable
---

{{HTMLSidebar("Global_attributes")}}

O [atributo global](/pt-BR/docs/Web/HTML/Global_attributes) **`contenteditable`** é um atributo enumerado indicando se o elemento deve ser editável pelo usuário. Se assim for, o navegador modifica seu widget para permitir a edição.

{{InteractiveExample("HTML Demo: contenteditable", "tabbed-shorter")}}

```html interactive-example
<blockquote contenteditable="true">
  <p>Edit this content to add your own quote</p>
</blockquote>

<cite contenteditable="true">-- Write your own name here</cite>
```

```css interactive-example
blockquote {
  background: #eee;
  border-radius: 5px;
  margin: 16px 0;
}

blockquote p {
  padding: 15px;
}

cite {
  margin: 16px 32px;
  font-weight: bold;
}

blockquote p::before {
  content: "\201C";
}

blockquote p::after {
  content: "\201D";
}

[contenteditable="true"] {
  caret-color: red;
}
```

O atributo deve ter um dos seguintes valores:

- `true` ou uma [string](/pt-BR/docs/Glossary/String) vazia, o que indica que o elemento é editável.
- `false`, o que indica que o elemento não é editável.

Se o atributo for aplicado sem um valor, como `<label contenteditable>Rótulo de Exemplo</label>`, seu valor é tratado como uma _string_ vazia.

Se esse atributo estiver faltando ou seu valor for inválido, seu valor é herdado de seu elemento pai: para que o elemento seja editável se seu pai for editável.

Observe que, embora seus valores permitidos incluam _true_ e _false_, este atributo é um enumerado e não um _[Booleano](/pt-BR/docs/Glossary/Boolean)_.

Você pode definir a cor usada para desenhar a inserção de texto {{Glossary("caret")}} com a propriedade {{cssxref("caret-color")}} do CSS.

## Especificações

{{Specifications}}

## Compatibilidade com navegadores

{{Compat}}

## Veja também

- [Tornando o conteúdo editável](/pt-BR/docs/conflicting/Web/HTML/Global_attributes/contenteditable)
- Todos os [atributos globais](/pt-BR/docs/Web/HTML/Global_attributes)
- {{domxref("HTMLElement.contentEditable")}} e {{domxref("HTMLElement.isContentEditable")}}
- A propriedade {{cssxref("caret-color")}} do CSS.
- [Evento de `input` - `HTMLElement`](/pt-BR/docs/Web/API/Element/input_event)
