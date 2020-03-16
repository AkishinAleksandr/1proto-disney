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
У тебя есть несколько сущностей в файле `cartoon`, одна из них является общей,чьи свойства повторяются в других.
Сделай доступныйми свойства и методы `Сartoon`  в `Disney Cartoon`  и  `DreamWorksCartoon` и убери лишнее.

> p.s. загляни в тесты

### Release 1

Давай разберемся с конструктором и наследованием. 
Определись что должно быть в `prototype` и от кого должны наследоваться твои функции киностудии.

> p.s. загляни в тесты

### Release 2

Мультики созданы для того чтобы их смотреть.

В файле `person` есть сущность `Person` у которой может быть имя( свойство `name` ) и список просмотренных фильмов( свойство `watchedMovies` ). А также метод просмотра мультика `watchMovie`, не забудь добавлять новые мультики в список уже просмотренных.

### Release 3
Если ты заглянешь в тесты `person-spec` то в последнем тестовом кейсе ты увидишь следующий код.

```sh
 let prettyString = 'The movies which Emma has watched:\n' + emma.watchedMovies;
```
Как ты думаешь что тут происходит ? 
Для начала поэкспериментируй с конкатенацией строки и массива. Со строкой все понятно, а что с [массивом](https://developer.mozilla.org/ru/docs/Web/JavaScript/Reference/Global_Objects/Array/toString) ? 

В данном примере у массива вызывается метод `toString`, который нам и надо переопределить. Но будь внимателен тебе нужно изменить метод конкретного массива, а не глобального объекта Array.

