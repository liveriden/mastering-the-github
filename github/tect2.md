---
    tags: [wiktionary-семантика]
    source: https://ru.wiktionary.org/wiki/%D1%81%D0%B5%D0%BC%D0%B0%D0%BD%D1%82%D0%B8%D0%BA%D0%B0
    created: 2023-05-22T06:47:50.205Z
---
# GitHub Flavored Markdown Spec

[линк-якорный — link-anchor](#линк-якорный---link-anchor)

.

.

.

.

## линк-якорный - link-anchor

```
[линк-якорный — link-anchor](#линк-якорный---link-anchor)
# линк-якорный - link-anchor

[link](#link)␠ ␠
# link

[link I](#link-I)␣␣
# link I␣␣

[link'I](#linkI)
# link'I

[link'I I:](#linkI-I)
# link'I I:

[link'I I: I](#linkI-I-I)
# link'I I: I

[link'I I: I I](#linkI-I-I-I)
# link'I I: I I
```
```html
It's also possible to create named custom anchors,
if for example you have a bunch of (sub-)headings with the same name.
To do this with a header insert an HTML tag:

<h4 id="login-optional-fields">
Optional Fields
</h4>

Then link to it by the ID attribute:

[see above](#login-optional-fields)

Also adding an anchor tag directly to the document works as well:

<a id="my-anchor"></a>

.

.

Также возможно создавать названные пользовательские якоря,
если, например, у вас есть куча (под-)заголовков с тем же именем.
Чтобы сделать это с заголовком, вставьте HTML -тег:

<h4 id="login-optional-fields">
Optional Fields
</h4>

Затем ссылка на него по атрибуту ID:

[see above](#login-optional-fields)

Также работает якорный тег непосредственно в документ:

<a id="my-anchor"></a>
```
```html
[see above](#login-optional-fields-2)
<div>
<h4 id="login-optional-fields-2">
Optional Fields
</h4>
</div>

[my-anchor](#my-anchor)
<div>
<a id="my-anchor">my anchor</a>
</div>
```

.

.

.

.
