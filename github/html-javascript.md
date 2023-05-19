аудиоплеер с плейлистом на JavaScript и HTML.

описание кода с примерами в формате разметки Markdown:
bbn
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Audio Player</title>
</head>
<body>
  <h1>Audio Player</h1>

  <audio id="audio-player" controls></audio>

  <ul id="playlist"></ul>

  <script type="text/javascript">
    // Создаем массив объектов, каждый из которых содержит информацию об одном треке
    var playlist = [
      {
        title: "Song 1",
        file: "https://live.radiospinner.com/nature-64"
      },
      {
        title: "Song 2",
        file: "https://live.radiospinner.com/nclssclwv-64"
      },
      {
        title: "Song 3",
        file: "https://radiorecord.hostingradio.ru/liquidfunk96.aacp"
      }
    ];
  
    // Получаем элементы DOM для аудиоплеера и списка воспроизведения
    var audioPlayer = document.getElementById("audio-player");
    var source = document.createElement("source");
    audioPlayer.appendChild(source);
    var playlistContainer = document.getElementById("playlist");

    // Создаем элементы списка воспроизведения на основе массива треков
    playlist.forEach(function(item) {
      var li = document.createElement("li");
      var link = document.createElement("a");
      link.setAttribute("href", item.file);
      link.textContent = item.title;
      // Добавляем обработчик клика на каждую ссылку списка воспроизведения,
      // чтобы установить новый источник для аудиоплеера и начать воспроизведение
      link.addEventListener("click", function(e) {
        e.preventDefault();
        audioPlayer.pause();
        source.setAttribute("src", item.file);
        audioPlayer.load();
        audioPlayer.play();
      });
      li.appendChild(link);
      playlistContainer.appendChild(li);
    });
  </script>
</body>
</html>
```

Этот код создает элемент `<audio>` с атрибутами `id="audio-player"` и `controls`, что означает, что он будет иметь стандартные элементы управления (кнопки "play", "pause", "volume" и т.д.). Также создаются пустой список воспроизведения `<ul>` с `id="playlist"`.

Далее создается массив объектов `playlist`, содержащий информацию о треках: название (`title`) и URL-адрес файла (`file`). Затем создаются элементы списка воспроизведения на основе этого массива, каждый из которых имеет ссылку с URL-адресом файла и обработчик клика, который устанавливает новый источник для аудиоплеера и начинает воспроизведение, когда пользователь выбирает трек из списка.

Наконец, создается элемент `<source>`, который будет использоваться для загрузки и воспроизведения аудиофайлов, и этот элемент добавляется как дочерний элемент к элементу `<audio>`.













































