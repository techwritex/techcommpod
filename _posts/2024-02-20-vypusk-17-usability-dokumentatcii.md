---
layout: post
title:  "Выпуск #17. Юзабилити документации"
date:   2024-02-20 01:00:00 +0000
keywords: documentation usability, юзабилити документации, удобство использования документации, тестирование юзабилити документации, usability testing, Jakob Nielsen, Джейкоб Нильсен, техкомпод, подкаст технического коммуникатора, Владимир Юсупов
summary: Жизненный цикл разработки любого продукта включает в себя этап тестирования. Более того, тестировать нужно не только функциональность, но и удобство использования (юзабилити). Документация, как продукт, не является исключением. В сегодняшнем выпуске затрагиваю такую тему, как тестирование удобства использования (usability testing) пользовательской документации.
categories: 
comments: false
episode: "Выпуск #17. Юзабилити документации"
---

Жизненный цикл разработки любого продукта включает в себя этап тестирования. Более того, тестировать нужно не только функциональность, но и удобство использования (юзабилити). Документация, как продукт, не является исключением. 

В сегодняшнем выпуске затрагиваю такую тему, как тестирование удобства использования (usability testing) пользовательской документации. 

<!--more-->

{% include player_frame.html src="https://techcommpod.s3.eu-north-1.amazonaws.com/pages/episode_017/index.html" %}

### Полезные ссылки

[«An Easy Way To Dramatically Improve Technical Documentation Quality» (George Eckel)](https://www.brighttalk.com/webcast/9273/601718)

[«Why You Only Need to Test with 5 Users» (Jakob Nielsen)](https://www.nngroup.com/articles/why-you-only-need-to-test-with-5-users/)

<br>

{% include podcast_platforms.html %}

{% include podcast_share_buttons.html %}

***

### Расшифровка выпуска

**00:00 - 03:40 Вступление** 

Добро пожаловать в подкаст технического коммуникатора Техкомпод!

С вами Владимир Юсупов - технический коммуникатор и ведущий данного подкаста.

Выпуск номер семнадцать.

Последние несколько недель ко мне регулярно обращается с вопросами один из ключевых пользователей аналитической системы, которую развивает и сопровождает наша команда. Сначала я не придал этому значения и подумал, что просто после новогодних каникул люди постепенно возвращаются в свое рабочее состояние и им требуется некоторая помощь в этом. Но через N-количество обращений я решил проверить портал с документацией, где даны подробные пояснения на все вопросы этого пользователя. 

И вот однажды, когда этот пользователь пришел с очередным вопросом, я уточнил у него, почему он не пользуется порталом с документацией, ведь там есть ответы практически на все вопросы касательно продукта (аналитической системы). Признаюсь ответ для меня был весьма неожиданный. 

<blockquote style="margin: 0; background: #F0F0F1;color: #333334;padding: 20px 30px;position: relative;border-left: 35px solid #DFDEDE;font-family: 'Lato', sans-serif;">
  <p style="margin: 0 0 16px;font-size: 20px;letter-spacing: .05em;line-height: 1.4;">Ты знаешь, вроде много материала разного. Видно, что вы его хорошо проработали, но как-то неудобно с этим материалом работать. И дело даже не в структуре, а, как бы это сказать, в упаковке и компоновке...</p>
  <footer>— <cite style="font-style: normal;font-weight: 300;">Один из ключевых пользователей аналитической системы</cite></footer>
</blockquote>

На меня будто ушат холодной воды вылили. Мы столько времени и сил потратили на подготовку документации, меняли и шлифовали формулировки и в итоге... «неудобно с этим материалом работать».

Тут у меня в голове загорелась лампочка.

Жизненный цикл разработки любого продукта включает в себя этап тестирования. Любая наша аналитическая система, отчеты, дашборды - словом, любой наш продукт - всегда тестируется пользователями при переносе новой разработки в продуктив (или продакшн). Но мы никогда не задумывались над тем, что пользовательскую документацию, которую мы создаем в процессе разработки продукта (или по ее завершению), тоже необходимо тестировать с привлечением именно пользователей продукта. Мы оформляли документацию так, как удобно было бы пользоваться ею нам - разработчикам, инженерам. И думали, что всем понятно. Но удобство для инженеров не равняется удобству для пользователям. Возможно, для вас это очевидно, но мы столкнулись с подобным явлением впервые.

И в сегодняшнем выпуске хочу затронуть такую тему, как тестирование удобства использования (или usability testing) документации. В частности, пользовательской документации.

{% include podcast_survey_banner.html %}

**03:41 - 07:52 Качественно не значит удобно**

Не знаю, как такое получается, но именно в тот момент, когда я обдумывал обозначенную проблему, я получил сообщение по электронной почте о вебинаре, на котором докладчик собирался как раз рассказать о значении тестирования документации в части удобства ее использования. Разумеется, я сразу же зарегистрировался на этот  вебинар.

В переводе на русский тема вебинара звучит следующим образом - «Простой способ значительно улучшить качество технической документации» («An Easy Way To Dramatically Improve Technical Documentation Quality»). Ссылка на него в описании выпуска. Если не ошибаюсь запись доступна по требованию, то есть сразу после регистрации. Докладчик - Джордж Эккл (George Eckel) - технический писатель с опытом работы около 25 лет и руководитель подразделения подготовки технической документации в компании ServiceNow.

Так вот, описание ситуации, с которой начинает докладчик, удивительным образом похожа на нашу. И в самом начале он задается тем же вопросом, что и мы.

<blockquote style="margin: 0; background: #F0F0F1;color: #333334;padding: 20px 30px;position: relative;border-left: 35px solid #DFDEDE;font-family: 'Lato', sans-serif;">
  <p style="margin: 0 0 16px;font-size: 20px;letter-spacing: .05em;line-height: 1.4;">Вы написали и отредактировали свой документ, провели техническую проверку. Зачем делать что-то еще?</p>
  <footer>— <cite style="font-style: normal;font-weight: 300;">Джордж Эккл (George Eckel)</cite></footer>
</blockquote>

И действительно, зачем? Такой простой и, вместе с тем, достаточно сложный вопрос. 

Затем Эккл приводит результаты анализа удовлетворенности порталом документации ServiceNow. И выяснилось следующее:
- более половины всех пользователей (54%) не нашли на портале документации нужную для них информацию,
- 43% пользователей сказали, что документация оказалась им не полезна. 

Эккл и его команда начали искать причину сложившейся ситуации. В процессе поиска они осознали, что если документация написана качественно - она содержит правдивую информацию, сформулирована понятными фразами и т.д. - это еще не значит, что этой документацией удобно пользоваться. Другими словами, они всегда тщательно проводили техническое ревью документации, но совсем не уделяли внимание анализу удобства пользования этой документацией. 

Более того, те, кто создавал документацию, очень хорошо знали продукт или, как минимум, имели понимание о том, как он работает, знали терминологию и т.д.

Ровно в той же ситуации оказались и наша команда. Мы всегда делали упор на качестве материала. Когда-то наша документация состояла из множества разрозненных документов. И на уровне отдельно взятого документа мы достаточно неплохо решали задачу по удобству использования, применяя весь арсенал Ворда. Но при этом уровень удобства пользования всей документацией (то есть всем массивом документов) стремился к нулю, так как приходилось отслеживать связи с другими документами, версии которых менялись, сами документы перемещались и т.д. Тут не то, что пользователям, самим инженерам приходилось несладко.

После того, как мы вывели нашу документацию на новую ступень эволюции, в Confluence, то были уверены, что теперь то документацией пользоваться удобно, количество обращений в поддержку уменьшится, так как пользователи прочитают нашу понятную документацию и самостоятельно найдут там ответы на свои вопросы, а мы, в свою очередь, займемся другими интересными задачами и не будем тратить время на консультации. Забавно конечно. Понимаю, что похоже на утопию какую-то.

**07:52 - 13:36 Исследования Нильсена-Нормана**

Далее Эккл упоминает результаты исследования удобства использования или юзабилити продукта Джейкоба Нильсена (Jakob Nielsen) и Дона Нормана (Don Norman), которые являются всемирно признанными экспертами в области дизайна. Так вот, согласно их исследованию, достаточно привлечь к тестированию всего пять пользователей, чтобы выявить до 85% проблем в дизайне продукта, или точнее в удобстве его использования. Именно на этих сведениях Эккл и делает акцент. Единственное, почему-то в своей презентации он говорит про 75%. Возможно, я не совсем верно его понял. Тем не менее...

Понятно, что перфекционизм - дело неблагодарное, но все же хочется выжать максимум - не 75% или 85%, а те же 100%. По крайней мере, хочется стремиться к такому результату. Поэтому мне стало любопытно, почему в этом исследовании ничего не говорится о достижении максимально возможных результатов. Оказывается, говорится. 

В общем, я пошел в первоисточник и выяснил следующее. Действительно, Джейкоб Нильсен уже с лохматого 1989 года говорит о пяти участниках в тестировании продукта. И не столь важно, что это за продукт - веб-сайт, интранет портал, десктопное или мобильное приложения и т.д. Соответственно, документация (в частности, портал с документацией) сюда вполне подходит. 

По Нильсену процесс тестирования должен быть итерационным. В каждой итерации должно быть не более пяти участников (или пользователей). Точнее может быть, но смысла в этом нет. Сейчас поясню почему.

По результатам своих исследований Джейкоб Нильсен построил график оптимального размера выборки для проведения качественного тестирования юзабилити. По оси абсцисс (или горизонтальной оси) представлено количество участников тестирования, а по оси ординат (или вертикальной оси) - обнаруженные проблемы в процентном выражении. В описании выпуска приведена ссылка на первоисточник, где как раз и представлен график.  

Если последовательно читать график слева направо, то первое, что бросается в глаза - при отсутствии участников тестирования мы не выявляем никакие проблемы с юзабилити. И это логично.

Привлечение к тестированию хотя бы одного участника позволяет выявить практически треть существующих проблем. 

Как правило, второй пользователь позволяет обнаружить в основном те же самые проблемы, что и первый, но в то же время второй пользователь может привнести новые знания о проблемах удобства работы с продуктом. 

Третий участник, с большой долей вероятности, позволит вам выявить ошибки первых двух участников и также сгенерирует новые знания о проблемах. 

И так далее. 

Но в определенный момент, а если быть точным, то после пятого пользователя вы будете получать все меньше и меньше новых сведений и практически не узнаете ничего нового. Поэтому Нильсен и говорит, что привлечение более пяти участников тестирования - просто трата времени.

Второе, что можно прочесть на графике - для обнаружения всех проблем в удобстве работы с продуктом потребуется всего 15 человек. Но здесь кроется еще одна хитрость. Может возникнуть соблазн сразу привлечь к тестированию 15 пользователей или же попросить одного пользователя протестировать удобство работы с продуктом 15 раз.

Смысл здесь как раз в небольших повторениях (итерациях). После того как первая итерация с пятью участниками поможет выявить до 85 % проблем с юзабилити, вы можете устранить эти проблемы и запустить повторное тестирование, чтобы выяснить помогло ли устранение ранее выявленных проблем или нет. Кроме того, при внедрении нового дизайна всегда есть риск появления новых проблем юзабилити, даже если старые были устранены.

Вторая итерация с новыми пятью участниками позволит обнаружить большинство из оставшихся 15% первоначальных проблем юзабилити, которые не были обнаружены на первом круге тестирования. Нильсен говорит, что результатом этого этапа является новый перечень проблем с юзабилити, но он гораздо меньше, чем после проведения первого тестирования. Как и на предыдущем шаге, вы скорее всего осознаете, что не все исправления сработали. К тому же, с большей долей вероятности, будут выявлены дополнительные проблемы. Для их устранения потребуется выполнить третью итерацию тестирования, которая поможет выявить и устранить порядка 2% первоначальных проблем.

Что же касается привлечение одного пользователя на 15 тестов, то этот вариант не подходит. Причина в том, что один пользователь скорее всего будет действовать по одной и той же схеме тестирования. Возникает большой риск быть введенным в заблуждение поведением одного человека, который выполняет действия по работе с продуктом. Большее количество участников позволяет получить представление о разнообразии поведения пользователей. 

**13:37 - 15:23 Принципы тестирования удобства документации**

Но вернемся к докладу Джорджа Эккла. В процессе тестирования удобного взаимодействия с документацией он выделяет следующие ключевые принципы:
1. Участники тестирования не должны быть знакомы с продуктом или документацией.
2. Участники тестирования выполняют задания только с помощью документации и без чьей-либо помощи.
3. Участники тестирования комментируют свои действия вслух.

По мнению Эккла, такой подход приближает тестирование к реальному сценарию по работе с продуктом. 

Далее докладчик в своей презентации приводит подробный скрипт выполнения тестирования документации, а также делится видеозаписью проведения реального теста.

В заключении Эккл говорит, что исследование юзабилити документации - это простой инструмент, который позволяет авторам (техническим писателям, инженерам и другим специалистам) обнаружить неявные для них проблемы с документацией. Ведь пользователям часто бывает достаточно трудно работать с нашей документацией, потому что у них нет общего понимания продукта, которое есть у нас, авторов этой документации.

Что тут сказать... Ни убавить, ни прибавить. Полностью согласен с докладчиком.

Теперь мы более серьезно подходим к тестированию нашей документации. Возможно, что когда-то все-таки наступит тот день, когда пользователи будут самостоятельно находить ответы на свои вопросы с помощью не только понятной, но и удобной документации.

**15:24 - 16:02 Заключение**

Спасибо, что прослушали сегодняшний выпуск. 

Очень любопытно узнать, каким образом вы тестируете свою документацию и тестируете ли вообще. Если у вас есть желание поделиться вашим опытом, напишите мне об этом. 

Напоминаю, что вы всегда можете ознакомиться с текстовой расшифровкой выпуска на сайте подкаста Техкомпод. 

С Вами был Владимир Юсупов. Подкаст технического коммуникатора Техкомпод. 

До встречи!


{% include podcast_subscribe_form_1.html %}