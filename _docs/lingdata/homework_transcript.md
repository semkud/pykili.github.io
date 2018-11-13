## Домашнее задание "Разработка фрагмента учебного корпуса", часть 2

### Расшифровка записей. Расстановка ударений и хезитаций

После выполнения первой части домашнего задания, у вас должно быть три файла (или больше, если фрагменты) вида:
* "Irkutsk_imp1960_1.mpg" - рассказ о себе
* "Irkutsk_imp1960_2.mpg" - чтение текста
* "Irkutsk_imp1960_3.mpg" - игра

#### Метаразметка записей

Добавьте [в таблице](https://docs.google.com/spreadsheets/d/1cyn1Fz7GlbsZ45xbuUgqcZ3c1pw4TRcsEQhj_Gky6-0/edit?usp=sharing) (если вы еще не..) данные о ВСЕХ говорящих, которые сказали более 10 слов подряд.
Если говорящих на записи несколько (в том числе это может быть вы), вставляйте строки сразу под названием файла. Обратите внимание, что ник (reo@) всегда должен заканчиваться знаком "собачки". 
Если какую-то информацию получить нельзя, оставляйте пустые клетки.

#### Расшифровка "Рассказа о себе"
Прослушайте запись, выберите 5 минут (подряд или фрагментами), наиболее удачно представляющих речь говорящего. Лучше, чтобы это было не начало и не самая последняя фраза. 
Расшифруйте запись так, как вы ее слышите, отражая все оговорки, неправильности, порядок слов, сниженную лексику, если есть. Пример расшифровки:
```
# time_begin = 3:55
aav@ там спрашивают фамилию-то / я сказала / Поликарпова ты с какого года? / ну это / родители сказали / 
с восемнадцатого нет / ты с семнадцатого я говорю / откуда / я с восемнадцатого //
sap@ а, ну да, ну да //
```
В начале (а также перед каждым новым фрагментом, если вы берете отдельные кусочки) вставьте отметку времени начала первой реплики. 
В начале каждой строки идет ник говорящего, после "собачки" ставится пробел.
Расшифровка ведется в стандартной русской орфографии, пунктуация может быть стандартная или со знаками больших и малых пауз 
(см. выше). Аббревиатуры записываются обычным образом (ср. ЦСКА). 
Разделение на абзацы может быть произвольным (по смыслу), реплика каждого следующего говорящего идет с новой строки.

Если текст в том или ином месте не удается разобрать, то используется тег [нрзб] ("неразборчиво"), который записывается так: `<noindex>[нрзб]</noindex>`. 
Когда говорят несколько человек одновременно и разобрать ничего не удается, нужно использовать ремарку `<noindex>[Говорят одновременно]<noindex>`. 
Одновременно звучащие реплики, если их удается разобрать, нужно записывать последовательно, друг за другом, порядок говорящих не важен. 
В случаях невербального общения (например, общий гул без ясно вычлененных реплик, смех, хмыканье) допустимо поставить ремарку, например, <noindex>[Все смеются]</noindex>, но увлекаться этим не нужно. 

Рекомендуем проигрывать записи в плейерах, поддерживающих замедленное воспроизведение, например, VLC.

#### Сохранение файла
Сохраните файл в текстовом виде, кодировка UTF-8, концы строк UNIX (LF), расширение файла `.transcript.txt` (например, Irkutsk_imp1960_1.transcipt.txt). Если вы работали в Word-е, перенесите файл в Notepad++ или его аналоги, чтобы не было проблем с форматами. 

#### Ударения в расшифровке
Воспользуйтесь [автоматическим LSTM-акцентуатором](https://linghub.ru/stress/), чтобы расставить ударения в расшифровке. 
Для этого загрузите файл на сайт (Choose file - Загрузить) и скопируйте акцентуированную запись в новый текстовый файл с расширением `acc.txt` (например, Irkutsk_imp1960_1.acc.txt).

##### Повторное прослушивание, редактирование и проверка ударений
Прослушивая текст повторно, вставьте все реплики, поддерживающие разговор (ага, ну), слова-паразиты (гм, ммм, эээ), недоговоренные слова (и тут она по... вышла), запинки (гово... сказала), междометия - т. е. все, что вы можете расслышать.
Все ударения должны соответствовать тому, как их поставил говорящий. Если человек сказал `торты'`, то необходимо поставить такое ударение. 
Обращайте особое внимание на сочетание нескольких односложных слов: `то е'сть vs. то' есть, во'т э'то vs. вот э'то`.
Бывают комплексы вообще без ударения, например, `_вот как бы это вот вам сказать_, неразу'мный` ("вот вам" точно будут без ударения, остальное нужно послушать).
Если ударения поставлены на комментариях или никах говорящих, удалите их оттуда. 

Выпишите слова, в которых наблюдается нестандартное ударение, заполнив [гугл-форму](https://docs.google.com/forms/d/e/1FAIpQLSeR0EeccjYIIF6rgs4LUD7VxL4zHtz6a3agHPiR6j5NsOBAWw/viewform?usp=sf_link).

Сохраните файл `..._1.acc.txt` и загрузите его в репозиторий LiveCorpus на ваш гитхаб (создайте таковой, если нужно).