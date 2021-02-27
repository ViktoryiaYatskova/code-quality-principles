# Качество кода

## Зачем?

Примеры плохого и хорошего проекта?

Что может случится?

// TODO: написать

## Общие правила

## 1. **DRY** — _dont repeat yourself_
or **DIE** — _Duplication Is Evil_

##

_Дублирование это зло!_

Принцип призывает Вас не повторяться при написании кода. Все что Вы пишите в проекте, должно быть определено только один раз.

### Примеры:

1. Циклы и функции (собственно сама цель этих сущностей в программировании - избежание дублирования логики)
```
const chips = ["corn", "pita", "potato", "tortilla"];

// non DRY code
console.log(chips[0]);
console.log(chips[1]);
console.log(chips[2]);

// DRY code
for ( let i = 0; i < chips.length; i++) {
    console.log(chips[i]);
}
```

// TODO: найти ещё примеров

<details>
    <summary>### Хочу знать больше:</summary>
    
    **History**: The principle was first introduced in the book The Pragmatic Programmer (by Andy Hunt, 1999). The principle itself was known and applied before this book came to life. However, the Pragmatic Programmer defined it precisely and put a name on it.
    
    In The Pragmatic Programmer, DRY is defined as
     &quot;Every piece of knowledge must have a single, unambiguous, authoritative representation within a system&quot;.
    
    Where, piece of knowledge, can be defined as either:
    
    Either, a precise functionality in the business domain of your application;
    
    Or an algorithm;
    
    // TODO: перевести на понятный русский
</details>

## **2. KISS** — _keep it short simple / keep it simple, stupid_


_Делайте вещи проще!_
 Порой наиболее правильное решение – это наиболее простая реализация задачи, в которой нет ничего лишнего.

// TODO: больше объяснений

Примеры: // TODO: написать

Хочу знать больше: // TODO: написать

2.
## **YAGNI** — _You ain"t gonna need it_

_ **Вам это не понадобится!** _
 Все что не предусмотрено техническим заданием проекта, не должно быть в нем.

// TODO: больше объяснений

Примеры: // TODO: написать

Хочу знать больше: // TODO: написать

1. **Комментарии**

// TODO: перевести

Explain code as needed, where possible.

Use comments to explain code: What does it cover, what purpose does it serve, why is respective solution used or preferred?

(This item is optional as it is not deemed a realistic expectation to always demand fully documented code. Mileage may vary heavily for HTML and CSS code and depends on the project"s complexity.)

1. **Action Items**

// TODO: перевести

Mark todos and action items with TODO.

Highlight todos by using the keyword TODO only.

Append a contact (username or mailing list) in parentheses as with the format TODO(contact).

Append action items after a colon as in TODO: action item.

| {# TODO(john.doe): revisit centering #}
<center\&gt;Test</center\&gt;
_<!--_ _TODO:_ _remove optional tags --\&gt;_
<ul\&gt;
<li\&gt;Apples</li\&gt;
<li\&gt;Oranges</li\&gt;
</ul\&gt; |
| --- |

1. **Хвостовые пробелы (Trailing whitespaces)**

Хвостовые проблемы являются излишними, к тому же они усложняют commit-изменения в Github (вы видите лишнюю строчку/символ изменений, не несущего смыслового изменения)

| _<!-- Not recommended --\&gt;_
<p\&gt;What?\_
_<!-- Recommended --\&gt;_
<p\&gt;Yes please. |
| --- |

## HTML + CSS

## Уровень 1:

- **Отступы**

Соблюдайте отступы в 2 пробела на каждый.

Не используйте tab-ы для отступов или смешанные отступы (tab и пробелы одновременно).

Почему?

Так как над проектами работает команда людей, то зачастую один исходный код проекта отображается в различных редакторах кода. Проблемы начинаются тогда, когда в одном файле используются разные методы идентации. Так как каждый редактор кода по разному отображает tab-отступ, то красивый файл в вашей IDE, может выглядеть совсем несуразно в другой.

[https://dev.by/news/otstupy-tab-ili-probel-programmist-proanaliziroval-milliard-faylov-i-nashyol-otvet](https://dev.by/news/otstupy-tab-ili-probel-programmist-proanaliziroval-milliard-faylov-i-nashyol-otvet)

| <ul\&gt;
<li\&gt;Fantastic
<li\&gt;Great
</ul\&gt; |
| --- |

| .example {
color: blue;
 } |
| --- |

- **Нижний регистр написания**

Весь код должен быть в нижнем регистре. Это касается всех HTML-имен, включая атрибуты, значения атрибутов, CSS-селекторы, CSS-свойства и значения.

| _<!-- Not recommended --\&gt;_
<A HREF=&quot;/&quot;\&gt;Home</A\&gt;
<!-- Recommended --\&gt;<img src=&quot;google.png&quot; alt=&quot;Google&quot;\&gt; |
| --- |

| _/\* Not recommended \*/_
**color** : **#E5E5E5** ;
_/\* Recommended \*/_
**color** : **#e5e5e5** ; |
| --- |

## HTML

## Уровень 1:

- **General Formatting**

// TODO: перевести

Use a new line for every block, list, or table element, and indent every such child element.

Independent of the styling of an element (as CSS allows elements to assume a different role per display property), put every block, list, or table element on a new line.

Also, indent them if they are child elements of a block, list, or table element.

(If you run into issues around whitespace between list items it"s acceptable to put all li elements in one line. A linter is encouraged to throw a warning instead of an error.)

| <blockquote\&gt;
<p\&gt;<em\&gt;Space</em\&gt;, the final frontier.</p\&gt;
</blockquote\&gt;
<ul\&gt;
<li\&gt;Moe
<li\&gt;Larry
<li\&gt;Curly
</ul\&gt;
<table\&gt;
<thead\&gt;
<tr\&gt;
<th scope=&quot;col&quot;\&gt;Income
<th scope=&quot;col&quot;\&gt;Taxes
<tbody\&gt;
<tr\&gt;
<td\&gt;$ 5.00
<td\&gt;$ 4.50
</table\&gt; |
| --- |

- **Document Type**

// TODO: перевести

Use HTML5.

HTML5 (HTML syntax) is preferred for all HTML documents: <!DOCTYPE html\&gt;.

(It"s recommended to use HTML, as text/html. Do not use XHTML. XHTML, as application/xhtml+xml, lacks both browser and infrastructure support and offers less room for optimization than HTML.)

Although fine with HTML, do not close void elements, i.e. write <br\&gt;, not <br /\&gt;.

- **HTML Quotation Marks**

When quoting attributes values, use double quotation marks.

Use double (&quot;&quot;) rather than single quotation marks ("") around attribute values.

| _<!-- Not recommended --\&gt;_
<a class="maia-button maia-button-secondary"\&gt;Sign in</a\&gt;
_<!-- Recommended --\&gt;_
<a class=&quot;maia-button maia-button-secondary&quot;\&gt;Sign in</a\&gt; |
| --- |

## Уровень 2:

- **Соблюдай семантику**

// TODO: перевести

Semantics

Use HTML according to its purpose.

Use elements (sometimes incorrectly called &quot;tags&quot;) for what they have been created for. For example, use heading elements for headings, p elements for paragraphs, a elements for anchors, etc.

Using HTML according to its purpose is important for accessibility, reuse, and code efficiency reasons.

| _<!-- Not recommended --\&gt;_
<div onclick=&quot;goToRecommendations();&quot;\&gt;All recommendations</div\&gt;
_<!-- Recommended --\&gt;_
<a href=&quot;recommendations/&quot;\&gt;All recommendations</a\&gt; |
| --- |

- **Multimedia Fallback**

// TODO: перевести

Provide alternative contents for multimedia.

For multimedia, such as images, videos, animated objects via canvas, make sure to offer alternative access. For images that means use of meaningful alternative text (alt) and for video and audio transcripts and captions, if available.

Providing alternative contents is important for accessibility reasons: A blind user has few cues to tell what an image is about without @alt, and other users may have no way of understanding what video or audio contents are about either.

(For images whose alt attributes would introduce redundancy, and for images whose purpose is purely decorative which you cannot immediately use CSS for, use no alternative text, as in alt=&quot;&quot;.)

| _<!-- Not recommended --\&gt;_
<img src=&quot;spreadsheet.png&quot;\&gt;
_<!-- Recommended --\&gt;_
<img src=&quot;spreadsheet.png&quot;alt=&quot;Spreadsheet screenshot.&quot;\&gt; |
| --- |

## По желанию:

- **HTML Line-Wrapping**

**B** reak long lines (optional).

While there is no column limit recommendation for HTML, you may consider wrapping long lines if it significantly improves readability.

When line-wrapping, each continuation line should be indented at least 4 additional spaces from the original line.

| <md-progress-circular md-mode=&quot;indeterminate&quot;class=&quot;md-accent&quot;
ng-show=&quot;ctrl.loading&quot;md-diameter=&quot;35&quot;\&gt;
</md-progress-circular\&gt;
<md-progress-circular
md-mode=&quot;indeterminate&quot;
class=&quot;md-accent&quot;
ng-show=&quot;ctrl.loading&quot;
md-diameter=&quot;35&quot;\&gt;
</md-progress-circular\&gt;
<md-progress-circular md-mode=&quot;indeterminate&quot;
class=&quot;md-accent&quot;
ng-show=&quot;ctrl.loading&quot;
md-diameter=&quot;35&quot;\&gt;
</md-progress-circular\&gt; |
| --- |

## CSS

## Уровень 1:

- **Единый стиль именования селекторов (классов / id)**

// TODO: расписать

- **ID and Class Naming**

Use meaningful or generic ID and class names.

Instead of presentational or cryptic names, always use ID and class names that reflect the purpose of the element in question, or that are otherwise generic.

Names that are specific and reflect the purpose of the element should be preferred as these are most understandable and the least likely to change.

Generic names are simply a fallback for elements that have no particular or no meaning different from their siblings. They are typically needed as &quot;helpers.&quot;

Using functional or generic names reduces the probability of unnecessary document or template changes.

| _/\* Not recommended: meaningless \*/_
**#yee-1901** {}

_/\* Not recommended: presentational \*/_
 .button-green {}
 .clear {}
_/\* Recommended: specific \*/_
**#gallery** {}
**#login** {}
 .video {}

_/\* Recommended: generic \*/_
 .aux {}
 .alt {} |
| --- |

## Уровень 2:

- **БЭМ**

- **Type Selectors**

Avoid qualifying ID and class names with type selectors.

Unless necessary (for example with helper classes), do not use element names in conjunction with IDs or classes.

Avoiding unnecessary ancestor selectors is useful for performance reasons.

| _/\* Not recommended \*/_
**ul**** #example** {}
**div**.error {}
_/\* Recommended \*/_
**#example** {}
 .error {} |
| --- |

## JS

- Волшебные числа (Magic numbers)
- Еще раз про дубликацию кода
  - Выноси одинаковую логику в функции

- Избегай вложенных функций
- Небольшие функции
- Одна функция - одно ~~действие~~

## GIT Commits

## Автоматизируй это!
 Или как упростить себе жизнь

// TODO: написать

- ESLint (Что это? Установка локально, интеграция в разные IDE)
- Хуки (precommit / prepush; что это? Как настроить)
- Интеграция job в Github repositories (Ура уже установлено, но можно рассказать, как это работает)
- SonarQube и другие инструменты