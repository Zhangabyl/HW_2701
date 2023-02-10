# Руководство по Git
Git - это консольная утилита, для отслеживания и ведения истории изменения файлов, в вашем проекте. Чаще всего его используют для кода, но можно и для других файлов. Например, для картинок
* --version - проверить текущую версию Git
* git config --global user.name «Ваше имя английскими буквами» - После установки необходимо «представиться» системе контроля версий. Это нужно сделать всего один раз, и git запомнит вас.
* git config --global user.email ваша почта@example.com - После установки необходимо указать почту системе контроля версий. Это нужно сделать всего один раз, и git запомнит ее.
* help - подсказки по популярным командам
* help название команды - подсказки по конкретной команде
* clear - очищает поле терминала
## Локальный репозитоий
### Команды

* init - создание локального репозитория
* add - добавление файла
* status - состояние репозитория
* commit - сохранение всех добавленных данных
* git commit --amend -m "Новое название коммита" - изменить имя последнего коммита
* diff - разница между текущими изменениями и последним коммитом
* checkout - переключение между коммитами и ветками
* checkout номер коммита - перейти к данному коммиту (достаточно указать первые 4-6 символов названия коммита)
* checkout master - вернуться на основную ветку
* log - показывает историю коммитов
* log --graph - показывает историю коммитов в виде графа/дерева
* branch - показать количество веток
* branch название ветки - создает новую ветку но не переходит на нее
* checkout -b название ветки - создает новую ветку и переходит на нее
* branch -d название ветки - удалить любую ветку
* merge название ветки - слить любую ветку с текущей
* clone ссылка - загружает все изменения, и пытается слить все ветки на локальном компьютере и в удаленном репозитории
* pull - Эта команда позволяет скачать все из текущего репозитория и автоматически сделать merge с нашей версией
* push - Отправить свою версию репозитория во внешний репозиторий. (**При первом её использовании нужна авторизация**)