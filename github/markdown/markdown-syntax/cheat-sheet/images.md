# пример как добавить изображение в markdown

Для включения изображений в Markdown-документах можно использовать следующий синтаксис:

```markdown
![Alt текст](путь_или_ссылка_на_картинку "Заголовок картинки")
```

Например, если у вас имеется файл `example.jpg`, расположенный в папке с вашим Markdown-файлом, то вы можете написать так:

```markdown
![](example.jpg)
```

Если же изображение находится по сети (в интернете), используйте полную или относительную ссылку на изображение:

```markdown
![Альтернативный текст для отображения](https://example.com/image.png "Заголовок картинки")
```

![example image](https://upload.wikimedia.org/wikipedia/commons/e/e8/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80.png "example image")

Изображение 120х120

```markdown
[<img src="https://example.com/image.png" width="120" height="120">]
```

<img src="https://upload.wikimedia.org/wikipedia/commons/e/e8/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80.png" width="120" height="120" alt="example image">

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/6/6a/PNG_Test.png/165px-PNG_Test.png" width="120" height="120" alt="example image">
