---
layout: post
title:  "Выпуск #10. Обзор Diataxis (системный подход к созданию технической документации) "
date:   2023-10-26 01:00:00 +0000
keywords: Diataxis, Daniele Procida, техкомпод, подкаст технического коммуникатора
summary: Diátaxis - подход структурирования и организации технической документации, который значительно упрощает работу с документацией как её разработчикам, так и читателям (пользователям). В  сегодняшнем выпуске представлен краткий обзор данного подхода.
categories: 
comments: false
episode: "Выпуск #10. Обзор Diataxis (системный подход к созданию технической документации)"
---

Diátaxis - подход структурирования и организации технической документации, который значительно упрощает работу с документацией как её разработчикам, так и читателям (пользователям). В  сегодняшнем выпуске представлен краткий обзор данного подхода.

<!--more-->

{% include player_frame.html src="https://techcommpod.s3.eu-north-1.amazonaws.com/pages/episode_010/index.html" %}

### Полезные ссылки

[diataxis.fr](https://diataxis.fr/)

[Daniele Procida](https://vurt.org/)

[Запись вебинара "Introducing the Diátaxis Approach to Technical Documentation"](https://www.brighttalk.com/webcast/9273/594742)

<br>

{% include podcast_platforms.html %}

{% include podcast_share_buttons.html %}

***

### Расшифровка выпуска

#### 00:00 - 01:56 Приветствие

Добро пожаловать в подкаст технического коммуникатора Техкомпод!

Меня зовут Владимир Юсупов. Я - технический коммуникатор и, по совместительству, ведущий данного подкаста.

На календаре 26 октября 2023 года. 

Выпуск номер деcять. Сегодня у нас небольшой юбилей. Очень радует, что аудитория подкаста постепенно растет. Пусть и маленькими шагами, но тем не менее увеличивается. Это конечно очень приятно. И придает силы для продолжения работы над подкастом.

Напомню, что одна из основных  тем подкаста - это разработка технической документации. 
Вчера принял участие в вебинаре Даниэле Просида (Daniele Procida) - создателя Diátaxis - подхода к организации технической документации. 

По свежим следам хочу сегодня поделиться своими мыслями и пониманием данной концепции, также с той целью, чтобы самому глубже разобраться в ней. Конечно же гораздо лучше всегда получать информацию из первоисточника, поэтому ссылку на запись вебинара я добавлю в описание к этому выпуску. Вебинар бесплатный, поэтому посмотрите, послушайте. Даниэле достаточно интересно рассказывает о своем детище. 

А пока послушайте мою вольную интерпретацию Diátaxis.

{% include podcast_survey_banner.html %}

#### 01:57 - 02:54 Концепция Diátaxis

Как я ранее уже сказал, Diátaxis - подход или концепция структурирования и организации технической документации. Данный подход становится всё более популярным среди техписателей, инженеров. Словом, всех тех, кто по долгу службы сталкивается с разработкой документации. 

Концепция строится на потребности пользователя в определённой информации о продукте в определённый момент времени. В своих заметках я уже неоднократно отмечал, что почти никто и никогда не читает документацию полностью. Как правило, из документации берется только какая-то часть информации, которая требуется для решения конкретной задачи прямо сейчас. Появится новая задача, начнется новый поиск и изучение информации опять же по этой конкретной задаче. И так далее.

#### 02:55 - 03:52 Обзор типов документации в Diátaxis

Так вот, исходя из потребностей пользователей, Даниэле в своей концепции предлагает разделение документации по четырем типам:

- **Туториалы** (*tutorials*) или обучающие материалы для описания пошаговых практических действий, в ходе выполнения которых происходит знакомство с продуктом. 
- **Руководства** (*how-to guides*) или пошаговые инструкции, которые ориентированы на решение конкретных задач при работе с продуктом.
- **Справочники** (*references*), которые используются для краткого и упорядоченного описания компонентов продукта. 
- **Объяснение** (*explanation*) - это верхнеуровневая информация, которая дает общее представление о продукте в целом.

#### 03:53 - 05:10 Взаимосвязь типов документации в Diátaxis

Кстати, интересна также взаимосвязь этих четырех типов.

Например, *объяснения* и *туториалы* используются для фундаментальных, (скажем так) исследовательских целей, когда необходимо получить общие сведения о продукте, не вдаваясь в детали. В свою очередь, *руководства* и *справочники* содержат прикладную информацию, которая используется непосредственно для выполнения рабочих задач.

При этом *объяснения* и *справочники* являются теоретической составляющей Diátaxis и не содержат никаких практических указаний, в отличие от *туториалов* и *руководств*, которые относятся к практической составляющей концепции Diátaxis.

Визуально разделение на типы технической документации и взаимосвязи между ними достаточно хорошо и понятно представлены в виде четырёх квадрантов плоскости. Как говорится, лучше один раз увидеть, чем сто раз услышать. Поэтому (опять же) рекомендую посмотреть вебинар или посетить сайт Diátaxis. Ссылки в описании.

#### 05:11 - 06:12 Туториалы

Теперь немного подробнее о каждом из озвученных типов.

Начнем с *туториалов*. 

Напомню, что это обучающие материалы для описания пошаговых практических действий, в ходе выполнения которых происходит знакомство с продуктом. Основная задача обучающих материалов (*туториалов*) - через успешное выполнение практических действий показать будущему пользователю, что он может достаточно успешно работать (или точнее, взаимодействовать) с продуктом. 

Другими словами, *туториалы* направлены на получение начальных практических навыков для дальнейшего использования продукта. Это если смотреть на *туториалы* с позиции человека, обучающегося. Для продукта же, *туториалы* являются своего рода конвертерами, которые преобразуют обучающихся в пользователей этого продукта. 

#### 06:13 - 07:08 Руководства

Далее идут *руководства* или как мы часто их называем “хаутушки”. 

Также напомню, что сюда можно отнести различные пошаговые инструкции, которые ориентированы на решение конкретных прикладных задач при работе с продуктом. 

Стоит отметить, что различные *руководства* нужны не только для того, чтобы помочь пользователям выполнить те или иные действия. Внушительный список “хаутушек” в документации помогает составить представление о возможностях продукта. Как правило, хорошо написанные руководства становятся самыми читаемыми или популярными разделами документации.

#### 07:09 - 08:04 Справочники

*Справочники* используются для одной единственной цели - краткого и упорядоченного описания компонентов продукта. В отличие от *туториалов* и “хаутушек”, которые отталкиваются от потребности пользователя, справочники определяются продуктом, который они описывают. 

В случае с программным обеспечением справочные материалы описывают само программное обеспечение - API, классы, функции и т.д. - и то, как их использовать. Хорошо и понятно составленные справочники позволяют пользователям легко и понятно взаимодействовать с продуктом. Опять же на примере программного обеспечения. Если API какого-то сервиса имеет понятное и подробное описание, то интеграция с таким сервисом потребует гораздо меньше времени и усилий. 

#### 08:05 - 09:26 Объяснение

И последний тип документации в парадигме Diátaxis - *объяснение*. 

Хотя всё-таки более правильно с него начинать. Но в контексте ознакомления и просто перечисления существующих типов порядок не столь важен. 

Итак, *объяснение* -  верхнеуровневая информация, которая дает общее представление о продукте в целом. С помощью документации данного типа пользователь просто проясняет свое понимание объекта документирования. 

Здесь не рассматриваются действия пользователя, как в туториалах и руководствах, и не добавляется подробное техническое описание, как в справочниках. Это скорее взгляд с высоты птичьего полета. В *объяснении* пользователь узнает, что это за продукт, для чего он нужен и т.д. При этом в отличие от предшествующих типов, документация типа объяснение может изучаться в отрыве от самого продукта. 

Основная задача - это познакомить пользователя с продуктом, не нагружая дополнительной, ненужной на конкретный момент времени, информацией.

#### 09:27 - 10:57 Заключение

Таким образом, мы сегодня вкратце рассмотрели подход в организации технической документации Diátaxis. Этот подход действительно упрощает как разработку и организацию документации специалистам, так и ее изучение пользователям. 

В то же время, Даниэле Просида отмечает, что Diátaxis не является истиной в последней инстанции. Необходимо прагматично подходить к его использованию. Нужно брать из этой концепции то, что каждый специалист по разработке технической документации считает нужным и полезным в конкретном проекте.

Спасибо, что прослушали этот выпуск от начала до конца. Если у Вас возникли вопросы, замечания или предложения, пишите мне. Заходите на мой сайт [techwritex.ru](https://techwritex.ru/). Там я периодически пишу заметки по техписьму и коммуникациям. И конечно же подписывайтесь на подкаст.

На этом у меня всё. До встречи!

С Вами был Владимир Юсупов. Подкаст технического коммуникатора Техкомпод. 

Пока!

{% include podcast_subscribe_form_1.html %}