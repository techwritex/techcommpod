---
layout: post
title:  "Выпуск #21. Инженеры-аналитики и dbt"
date:   2024-09-19 01:00:00 +0000
keywords: инженер-аналитик, dbt, роли команды данных, роли дата-команды, техкомпод, подкаст технического коммуникатора
summary: Мир данных уже не тот. Как и всё вокруг нас меняется с немыслимой скоростью, мир данных очень сильно изменился, особенно за последние несколько лет. Если 10–15 лет назад тенденция была такова, что от специалиста требовалось наличие широкого спектра навыков, то ситуация поменялась кардинальным образом – сейчас в тренде узкая специализация. Это приводит к некоторым изменениям в существующих профессиях, а также к появлению новых профессий. Об одной из таких профессий в сегодняшнем выпуске.
categories: 
comments: false
episode: "Выпуск #21. Инженеры-аналитики и dbt"
---

Мир данных уже не тот. Как и всё вокруг нас меняется с немыслимой скоростью, мир данных очень сильно изменился, особенно за последние несколько лет. 

Если 10–15 лет назад тенденция была такова, что от специалиста требовалось наличие широкого спектра навыков, то ситуация поменялась кардинальным образом – сейчас в тренде узкая специализация. Это приводит к некоторым изменениям в существующих профессиях, а также к появлению новых профессий. 

Об одной из таких профессий в сегодняшнем выпуске.

<!--more-->

{% include player_frame.html src="https://techcommpod.s3.eu-north-1.amazonaws.com/pages/episode_021/index.html" %}

### Полезные ссылки

Сайт инструмента (в том числе, документация) - www.getdbt.com

Книга «Data Engineering with dbt: A practical guide to building a cloud-based, pragmatic, and dependable data platform with SQL» (Roberto Zagni)

Книга «Fundamentals of Analytics Engineering: An introduction to building end-to-end analytics solutions» (Dumky De Wilde, Fanny Kassapian, Jovan Gligorevic, Juan Manuel Perafan, Lasse Benninga, Ricardo Angel Granados Lopez, Taís Laurindo Pereira)

<br>

{% include podcast_platforms.html %}

{% include podcast_share_buttons.html %}

***

### Расшифровка выпуска

**00:00 - 02:51 Вступление** 

Добро пожаловать в подкаст технического коммуникатора Техкомпод!

С вами Владимир Юсупов – технический коммуникатор и ведущий данного подкаста.

Выпуск номер двадцать один.

Мир данных уже не тот. Как и всё вокруг нас меняется с немыслимой скоростью, мир данных очень сильно изменился, особенно за последние несколько лет. Если 10–15 лет назад тенденция была такова, что от специалиста требовалось наличие широкого спектра навыков, то ситуация поменялась кардинальным образом – сейчас в тренде узкая специализация. Постараюсь пояснить на своём примере из сферы Business Intelligence (BI).

Когда я начинал свой путь BI-консультанта в 2009 году, то мы выполняли весь комплекс задач касательно хранилищ данных:

- проектирование хранилища,
- разработка объектов хранилища
- подготовка данных в системах-источниках (по крайней мере, в части формирования требований для экспорта данных),
- загрузка данных в хранилище,
- преобразование данных по заданной бизнес-логике,
- формирование отчётности и дашбордов,
- обучение пользователей и т.д.

Что же мы видим сейчас?

Весь объём работы, который выполнял раньше один BI-консультант (или BI-разработчик, BI-инженер), разделён, как минимум, на «троих»:

- инженер по обработке данных (data engineer),
- аналитик данных (data analyst),
- инженер-аналитик (analytics engineer).

Инженеры по обработке данных и аналитики данных всем хорошо известны и у всех на слуху (по крайней мере, у тех, кто имеет отношение к индустрии), а вот инженеры-аналитики появились буквально несколько лет назад. Если не ошибаюсь, эта профессия впервые публично была упомянута в самом начале 2019 года и объединила под собой определенную группу специалистов. И с тех самых пор сообщество инженеров-аналитиков постоянно увеличивается. Популяризации новой  профессии способствует компания dbt Labs. 

Вот про эту новую роль в мире данных и продукт компании dbt Labs я хочу немного рассказать в сегодняшнем выпуске.

{% include podcast_survey_banner.html %}

**02:52 - 04:01 Кто же такие инженеры-аналитики?** 

Так кто же такие инженеры-аналитики?

Думаю, интуитивно понятно, что это некий специалист, который сочетает в себе навыки и знания инженеров и аналитиков. По сути так и есть. Инженеров-аналитиков можно назвать связующем звеном между бизнес-заказчиком и командой по разработке платформ данных. Инженеры-аналитики, в первую очередь, четко понимают потребности бизнеса, погружены в бизнес-тематику. И это у них от аналитиков. Но при этом инженеры-аналитики принимают непосредственное участие в процессе создания и поддержания платформ данных. И здесь важный момент – в части преобразования нужных наборов данных, которые удовлетворяют потребности бизнеса. 

**04:02 - 09:04** 

Итак, давайте сравним озвученные ранее роли специалистов по работе с данными относительно основных задач по созданию хранилищ данных (или платформ данных).




- Настраивает и обеспечивает бесперебойную загрузку данных (интеграцию) из систем-источников в хранилище
- Сосредотачивается на поддержке инфраструктуры доставки данных, а не на анализе самих данных
- Проектирует (моделирует) хранилище данных
- Преобразует данные из систем-источников по заданной бизнес-логике для проведения анализа конечными пользователями (аналитиками и/или бизнес-пользователями) с применением принципов разработки программного обеспечения
- Погружается как в техническую сторону обработки данных, так и в потребности бизнеса
- Оформляет и поддерживает документацию по хранилищу (платформе данных)
- Отвечает за визуализацию данных (отчёты, дашборды)
- Тесно взаимодействует с бизнес-пользователями
- Глубоко погружается в потребности бизнеса

<table style="border: 1px solid #ddd; border-collapse: collapse; text-align: left; width: 100%;">
    <caption style="color: #6c6c6c; text-align: right;">Роли современной дата-команды</caption>
    <colgroup>
    <col width="33%" />
    <col width="34%" />
    <col width="33%" />
    </colgroup>
    <thead>
        <tr class="header">
            <th style="border: 1px solid #ddd; text-align: left; padding: 15px;">Инженер по обработке данных (data engineer)</th>
            <th style="border: 1px solid #ddd; text-align: left; padding: 15px;">Инженер-аналитик (analytics engineer)</th>
            <th style="border: 1px solid #ddd; text-align: left; padding: 15px;">Аналитик данных (data analyst)</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td markdown="span" style="border: 1px solid #ddd; text-align: left; padding: 15px;">
                - Настраивает и обеспечивает бесперебойную загрузку данных (интеграцию) из систем-источников в хранилище<br>
                - Сосредотачивается на поддержке инфраструктуры доставки данных, а не на анализе самих данных<br>
            </td>
            <td markdown="span" style="border: 1px solid #ddd; text-align: left; padding: 15px;">
                - Проектирует (моделирует) хранилище данных<br>
                - Преобразует данные из систем-источников по заданной бизнес-логике для проведения анализа конечными пользователями (аналитиками и/или бизнес-пользователями) с применением принципов разработки программного обеспечения<br>
                - Погружается как в техническую сторону обработки данных, так и в потребности бизнеса<br>
                - Оформляет и поддерживает документацию по хранилищу (платформе данных)<br>
            </td>
            <td markdown="span" style="border: 1px solid #ddd; text-align: left; padding: 15px;">
                - Отвечает за визуализацию данных (отчёты, дашборды)<br> 
                - Тесно взаимодействует с бизнес-пользователями<br>
                - Глубоко погружается в потребности бизнеса<br>     
            </td>
        </tr>
    </tbody>
</table>

Таким образом, инженеры-аналитики находятся на пересечении инженерии данных и аналитики. 

**09:05 - 10:17 Зачем же нужны инженеры-аналитики?** 

Возникает простой вопрос – зачем же нужны инженеры-аналитики, если эту работу уже выполняют другие специалисты?

Дело здесь в следующем. Об этом я упомянул ранее. Узкая специализация.  

Проблема в том, что дата-инженеры в основном заняты разработкой и поддержкой инфраструктуры по экстракции (извлечению) данных из различных источников и загрузки этих данных в целевые системы (хранилища данных). И это их специализация. В связи с этим, дата-инженеры не всегда могут уделить должное внимание проектированию моделей данных. Конечно они выполняют активности по моделированию, но часто сталкиваются с проблемой качества, во-первых из-за отсутствия времени на эту задачу, а во-вторых, нежелания вникать в потребности бизнеса. Здесь можно резонно сказать, что этим должны заниматься аналитики, которые погружены в бизнес-потребности и плотно общаются с заказчиками. Но, скажем так, техническая работа  аналитиков данных ограничивается созданием дашбордов и отчётности. Они не всегда (возможно, никогда) имеют достаточного представления о сложных процессах преобразования данных. Аналитики данных получают готовые наборы данных для своей дальнейшей работы. Если какие-то рассчитанные метрики или показатели оказываются неверными, то аналитики данных, как правило, не могут внести исправления оперативно и это приводит к тому, что заказчики могут просто потерять доверие к данным. В конечном итоге страдает бизнес, это сказывается на эффективности принятия различных управленческих решений, основанных на данных, точнее некорректных данных. 

Здесь и появляется тот самый инженер-аналитик, который, как было замечено ранее, погружен в бизнес-потребности и занимается именно моделированием и трансформацией (преобразованием) данных. Этот специалист может оперативно сориентировать о том, как и почему данные преобразованы, а также, в случае необходимости, оперативно, насколько это возможно, может внести соответствующие исправления в процесс трансформации данных. При этом не отвлекаются дата-инженеры от своей работы и аналитики тоже заняты своим делом.

Есть ещё, кстати, один момент, который следует отметить в качестве одной из причин появления и распространения новой роли в команде данных. Причина эта – сдвиг от ETL к ELT. Сейчас немного поясню термины и их суть, на тот случай, если вы не сталкивались с ними. 

ETL – Extract, Transformation, Load – процесс, при котором данные извлекаются из различных источников, преобразуются сразу после извлечения и уже потом загружаются в хранилище. Этот подход применялся и применяется с той целью, чтобы снизить расходы на содержание хранилища. Данный подход был долгое время стандартом в индустрии. И здесь дата-инженеры являлись, можно сказать, владельцами всего процесса, в свою очередь, аналитики имели только некоторое представление о логике преобразования данных без технических подробностей. 

Появление и развитие, в основном, облачных решений способствовало созданию масштабируемых и экономически эффективных систем вычислений и хранения данных. Проще говоря, хранилища стали больше и дешевле. Преобразование данных до загрузки в хранилище перестало быть актуальным. Можно сразу загружать данные из источников, а затем уже в самом хранилище выбирать необходимые данные и преобразовывать их по нужной бизнес-логике. Такой процесс стал называться ELT – Extract, Load, Transformation – извлечение, загрузка, преобразование. 

Таким образом, в ELT-подходе дата-инженеры фокусируют свои усилия на извлечении и загрузке данных, а инженеры-аналитики – на преобразовании. И затем предоставляют аналитикам готовые наборы данных для дальнейшей визуализации через отчётность и дашборды. 

Итак, думаю, разобрались с инженерами-аналитиками, кто они и зачем. 

**10:18 - 17:31 Основной инструмент инженеров-аналитиков** 

Теперь немного расскажу об инструментах, точнее об одном из инструментов, с которым работают инженеры-аналитики. 

Как я сказал ранее, одним из игроков в мире данных на данный момент, который занимается популяризацией новой профессии, является компания dbt Labs. Изначально компания называлась Fishtown Analytics и вела деятельность в сфере консультирования по работе с данными. Эта компания является разработчиком продукта, ставшего, пожалуй, стандартом и обязательным инструментом в арсенале инженеров-аналитиков. Продукт называется dbt (data build tool), а компанию переименовали в dbt Labs. 

Замечу, что название инструмента пишется именно строчными буквами (dbt). Потому как написание DBT прописными (заглавными) буквами является аббревиатурой системы когнитивно-поведенческой терапии, предназначенной для людей с пограничным расстройством личности. Поэтому если будете гуглить, будьте внимательны. 

Если вкратце, то dbt (тот который инструмент, а не система терапии) позволяет инженерам-аналитикам (да и любым специалистам по работе с данными) преобразовывать и тестировать данные, а также создавать документацию на хранилище. dbt входит в, так называемый, современный набор технологий по работе с данными (modern data stack).

Основной парадигмой dbt является то, что трансформация данных должна выполняться по шагам, которые делают преобразования прозрачными и понятными. Если использовать терминологию создания хранилищ данных, то эти шаги называются слоями. Например, в dbt принято использовать следующие слои: Staging, Intermediate и Marts. 

Расскажу вкратце о каждом из слоев.

Staging – слой первичных данных,  на котором практически не выполняются никакие преобразования данных. Здесь повторяются источники данных один к одному. Основная задача этого слоя – подготовка фундамента для построения хранилища. Максимум, что можно здесь сделать – провести небольшую очистку и подготовку таблиц для дальнейшего использования. Например, переименовать некоторые поля исходных таблиц, привести типы каких-то полей и т.д. Агрегирование и джоины – задачи других слоев.

Intermediate – промежуточный слой – это то место, где модели исходного слоя объединяются и создают новый разрез данных в соответствии с логикой и потребностями бизнеса. Именно здесь выполняются джоины и агрегирование, обеспечивается качество и целостность данных.

Marts – исходя из названия, означает витрины. На слое витрин происходит  формирование сущностей, каждая из которых предназначена для определенной цели. Это могут быть справочники, метрики или какие-то показатели в целом. Например, заказчики, оплата и т.д.

Все эти сущности, да в принципе практически все объекты в dbt называются моделями, которые являются отдельными SQL-файлами, написанными с помощью оператора SELECT. Это кстати, одно из преимуществ dbt. Вся работа ведется в SQL. Всё-таки каждый специалист по работе с данными должен знать SQL (как минимум, на уровне написания SELECT-ов). Нет необходимости изучать новый язык программирования для использования инструмента. Но кстати, здесь же к преимуществам dbt можно отнести расширение функциональности SQL с помощью шаблонизатора Jinja, который дает возможность применять условия (IF) и циклы (FOR) в моделях, а также многократно переиспользовать созданные модели.

Раз уж я упомянул о некоторых преимуществах dbt, то перечислю еще несколько положительных моментов.

dbt прекрасно интегрируется с Git. При этом каждый разработчик может иметь свою собственную песочницу с конфигурацией целевой базы данных и схемы. Условно говоря, при создании модели в скрипте пишется просто select * from source('имя источника','таблица источника'). Другими словами, код не завязан на конкретные наименования объектов определенного разработчика. Эти конкретные объекты подставляются в момент компиляции кода. Таким образом, любой новый код можно легко и безопасно слить с основной веткой в git и затем выполнить другими участниками команды. То есть исключается вероятность случайной перезаписи объектов.

Продолжая тему преимуществ и всколь упомянутого тестирования. В dbt существует несколько способов настройки проверок качества данных. Прямо из коробки инструмент позволяет легко создавать проверки целостности данных (null, уникальность, внешние ключи, допустимый диапазон значений), когда вы документируете конкретную модель. А также имеется возможность создания пользовательских тестов данных, которые определяются бизнес-логикой. Опять же всё это выполняется в виде оператора SELECT. 

Также в арсенале dbt имеется функциональность по автоматическому созданию документации в виде статического сайта, на котором представлена подробная информация о существующих моделях, а также связанных с ними объектов источников данных. Более того, dbt строит направленный ациклический граф (DAG - directed acyclic graph) на основе взаимозависимостей между моделями, который определяет порядок выполнения моделей и обеспечивает наглядную визуализацию зависимостей. Таким образом, с помощью графа всегда можно легко и быстро проследить потоки данных от источника до цели и наоборот.

Отмечу также, что dbt поставляется в двух вариантах:
- Коммерческая версия, которая называется dbt Cloud
- Open-source версия, которая называется dbt Core

Пожалуй, основным отличием между версиями является то, что облачное решение имеет веб-интерфейс. Для многих этот вариант использования более удобный. В бесплатной же версии предполагается работа только с помощью командной строки. В остальном возможности практически одинаковые. Есть отличия, но сегодня их касаться не будем.

В общем, dbt – это мощный фреймворк для аналитиков и инженеров, а также новой роли инженеров-аналитиков, позволяющий создавать, тестировать и документировать хранилища данных, используя только SQL. 

**17:32 - 18:41 Источники информации об инженерах-аналитиках и dbt**

На сегодня это, пожалуй, всё, что я хотел рассказать в качестве небольшого введения в тему новой роли дата-команды, а также инструментов, с которыми сейчас работают специалисты по работе с данными. Продолжу освещение этой темы в последующих выпусках.

Но если у кого-то есть желание прямо сейчас подробнее разобраться с dbt и почитать об инженерах-аналитиках, то могу порекомендовать те источники, с которыми я лично ознакомился. Можно погуглить и найти достаточно много материала по этим темам.

Итак, мой первый источник – сайт самого инструмента dbt с описанием и подробной документацией (getdbt.com).

Второй источник – книга Роберто Загни Data Engineering with dbt. 

Третий источник – книга группы товарищей (по-моему 7 авторов) Fundamentals of Analytics Engineering. 

Обе книги на английском языке. В описании и расшифровке выпуска продублирую названия упомянутых источников.

**18:42 - 19:05 Заключение**

Благодарю, что прослушали этот выпуск. 

Напоминаю, что вы всегда можете ознакомиться с текстовой расшифровкой на сайте подкаста. 

С Вами был Владимир Юсупов. Подкаст технического коммуникатора Техкомпод. До встречи! 


{% include podcast_subscribe_form_1.html %}