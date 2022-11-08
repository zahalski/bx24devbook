# Bitrix24: Книга разработчика

Это руководство, которое рассматривает разработку под Битрикс24 как фреймворк с учетом аспектов применения его в законченном продукте.
Целью данного руководства является:
* Систематизация знаний в области API Битрикс24
* Упрощение изучения платформы для новых разработчиков

Руководство не ставит цели заменить существующие курсы связанные с Битрикс24 и платформой Bitrix Framework, но стараемся дополнить их актуальной информацией которая поможет в работе. Мы надеемся что каждый специалист найдет в ней что-то полезное.


## Как принять участие?

Существует несколько способов принять участие в разработке документации:

* В issue писать недостающе темы
* Проводить review, исправть орфографические и другие ошибки
* Писать статьи

Все способы перечислены от наименьшего к наибольшему вкладу, мы будем благодарны за любой вклад.

## Как написать первую статью?

Процесс написания статьи с точки зрения технического писателя выглядит следующим образом:

1. Зарегистрироваться на github, скачать и установить необходимое ПО.
2. Клонировать репозиторий документации к себе.
3. Написать или отредактировать статью. Проверить результат.
4. Оформление pull request с предложением.

### Подготовка и необходимое ПО

Файлы книги описаны в формате [Markdown](https://en.wikipedia.org/wiki/Markdown). Ознакомьтесь с наиболее популярной спецификацией - [GitHub Flavored Markdown Spec](https://github.github.com/gfm/). Мы стараемся ориентироваться на нее.

Для генерации документации мы используем [Daux.io](http://daux.io/), который потребуется установить на ПК для визуального осмотра документации.
Требования `daux`:
- PHP 8.0+
- Установленные модули: 
	- php-mbstring
	- php-xml
	- php-intl

### Клонирования репозитория

На текущий момент, мы не ведем работу с ветками (`branch`) github, поэтому вам придется [форкнуть репозиторий](https://docs.github.com/en/get-started/quickstart/fork-a-repo) к себе.
Возможно мы еще вернемся к обсуждению этого вопроса, но не сегодня.

### Внесение изменений

После того как готово, вы можете вносить изменения.
Вы как автор вольны вносить любые изменения, но старайтесь придерживаться следующих рекомендаций:
1. Используйте терминологию 1С-Битрикс, но не боятесь если вы придумаете что-то свое.
>Например, стандартная документация слабо описывает сущность "смарт-процесса" и в разных ее частях можно встретить как под этим термином даже в рамках одного документа понимаются разные вещи. Старайтесь избегать подобного
2. Описывайте максимально доходчиво.
>Мы не ставим ограничений на уровень читателей, понятно должно быть всем от новичков до профессионалов.
3. Начните с малого
>Лучше охватить наиболее емко небольшую часть, чем большую тему по верхам.

### После внесения изменений

Когда ваше творческая деятельность закончена, необходимо провести проверку.
Перейдите в корень проекта и выполните комманду
```php
daux generate
```

На выходе в директории static будет сгенерирована документация.
Проверьте ее визуально, при необходимости внесите исправления и повторите этот шаг.

### Оформление pull request

Теперь когда у вас готовы ваши изменения, вы можете поделиться ими с сообществом.
Для этого загрузите измнения из вашего локального репозитория на github. Далее перейдите в проект `gromdron/bx24devbook` и создайте [pull request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request).

