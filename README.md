# Disney 🧚
### Proto and prototype and bind
  ![screenshot](readme-assets/349186.jpg).

### Release 0

В папке `src` у тебя есть два файла `cartoon` и `person`. В первую очередь ознакомься с этими файлами и изучи содержимое. 
```sh
function Cartoon(title, year, forChildren = true, beginning = 'Long, long ago...') {
  this.title = title;
  this.year = year;
  this.forChildren = forChildren;
  this.beginning = beginning;
}
```
У тебя есть одна сущность, с свойствами, которые повторяются.
Сделай доступныйми свойства и методы `Сartoon`  в `Disney Cartoon`  и  `DreamWorksCartoon` и убери лишнее.
### Release 1
Давай разберемся с конструктором и наследованием. 
Определись что должно быть в `prototype` и от кого должны наследоваться твои функции киностудии.

> p.s. загляни в тесты

### Release 2

Мультики созданы для того чтобы их смотреть. В файле `person` есть сущность `Person` у которой может быть имя и список просмотренных фильмов,а также метод просмотра этого мультика.

### Release 3
Если ты заглянешь в тесты `person-spec` то в последнем тестовом кейсе ты увидишь следующий код.

```sh
 let prettyString = 'The movies which Emma has watched:\n' + emma.watchedMovies;
```


