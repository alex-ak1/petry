# Сети Петри (petry net)
Всякие <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%B5%D1%82%D1%8C_%D0%9F%D0%B5%D1%82%D1%80%D0%B8">сети Петри</a>

Базовая сеть Петри - граф, состоящий из чередующихся узлов и переходов. В каждом узле может содержаться от 0 до бесконечности фишек.
Переход возможен, если у всех входных узлов есть достаточное количество фишек. Переход считается атомарной операцией.

С помощью сети Петри можно симулировать такие вещи как:
- всякие примитивы синхронизации - <a href="https://github.com/alex-ak1/petry/wiki/petry1">семафоры, мьютексы</a> и так далее.
- <a href="https://github.com/alex-ak1/petry/wiki/petry2"> логические булевы операции</a>.

Для моделирования сетей можно использовать следующую программу: http://pipe2.sourceforge.net/
# организация сети
Сеть состоит из следующих частей:
- список узлов. содержать фишки.
- список переходов. фишки не содержат, но описывают откуда и куда они идут.
-- входные и выходные связи. 

Каждый переход имеет несколько входных связей и выходных (несколько это в том числе 0). Все связи входные отходят от узла и заканчиваются переходом, а выходные идут от перехода к узлу.

Каждая связь может иметь не единичную кратность, а большую, к примеру требуется 3 фишки, чтобы совершить переход.

Связей между переходом и переходом быть напрямую не может, также как и связь между узлом и узлом.

Для визуализации можно добавить во все эти элементы различные украшения - цветные фишки (может быть полезно и для визуализации, и для логики), цветные узлы и переходы, координаты рисования узлов на экране и так далее.


