# Задача "Чистый код S1E1"

| Дата выдачи | Deadline         | Folder name     | Branch name     |
| ----------- | ---------------- | --------------- | --------------- |
| 23.03.2021  | 30.03.2021 23:59 | clean-code-s1e1 | clean-code-s1e1 |

## Task 2. Описание: 

![image](https://user-images.githubusercontent.com/8201843/111080709-d1289200-8510-11eb-861c-c39de6d99691.png)

Перед вами небольшое одностраничное веб-приложение.
Ваша задача - это навести порядок внутри файлов кода (_рефакторинг_) согласно следующим руководствам:
 [тут](https://github.com/ViktoryiaYatskova/code-quality-principles/blob/main/html-and-css.md)
 и [тут](https://github.com/ViktoryiaYatskova/code-quality-principles/blob/main/html-and-css-extended.md) (только html и css файлы). 
При этом функционал приложения должен остаться все еще рабочим после ваших изменений.

## Требования к выполнению

**Внимание!** Задача не может быть принята, если условия ниже не выполнены

- Используйте личный ПУБЛИЧНЫЙ репозиторий в GitHub для выполнения данного задания
- Один git-коммит должен содержать изменения согласно одному пункту из руководств.
(можно несколько коммитов на 1 пункт руководства, но не наоборот).
Обязательно укажите, какой пункт покрывают изменения в данном коммите.
- Коммит-сообщения должны быть составлены согласно [следующим правилам](https://github.com/ViktoryiaYatskova/code-quality-principles/blob/main/commits.md)

_Пример:_
```
fix: add Html5 DOCTYPE tag according to rule 2.2 in html-and-css.md
refactor: adjust HTML-formatting according to rule 2.1 in html-and-css.md
```

- Весь функционал приложения должен исправно работать после ваших изменений, а именно:

    - Добавление нового элемента в список задач "TODO"
    - Редактирование элемента в списке задач "TODO"
    - Удаление элемента из списка задач "TODO"
    - Установка элемента в статус завершенного и перенос в список "COMPLETED" через checkbox

    - Удаление элемента из списка "COMPLETED"
    - Редактирование элемента из списка "COMPLETED"
    - Установка элемента в статус незавершенного и перенос в список "TODO" через checkbox

- Внешний вид приложения не изменился
- Анимация на кнопке удаления работает

## Критерии оценки

**Максимальный балл за задание +45**

- Каждый из 15 пунктов [первого](https://github.com/ViktoryiaYatskova/code-quality-principles/blob/main/html-and-css.md) руководства соблюден:
    - +2 за каждое ПОЛНОСТЬЮ выполненное правило
    (т.е. правило должно быть соблюдено для всего документа, а не только для кусочка кода)
- Каждый из 3 пунктов [расширенного руководства](https://github.com/ViktoryiaYatskova/code-quality-principles/blob/main/html-and-css-extended.md) соблюден: 
    - +5 за каждое ПОЛНОСТЬЮ выполненное правило

## Ключевые навыки
- Написание чистого, читабельного кода

## Материалы:
- "Чистый код", Роберт Мартин
- [Википедия: Coding Conventions](https://en.wikipedia.org/wiki/Coding_conventions)

[Документ для вопросов](https://docs.google.com/spreadsheets/d/1lgzmc72mKCmYvHimvqBNENgKJuXMON8q1f1s4GEnEVI/edit?usp=sharing)

## Cross-check
- форма для проверки задания: https://clean-code-s1e1-cross-check.netlify.app/
- инструкция по проведению cross-check: https://docs.rs.school/#/cross-check-flow