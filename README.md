# Сети Петри (petry net)
Всякие <a href="https://ru.wikipedia.org/wiki/%D0%A1%D0%B5%D1%82%D1%8C_%D0%9F%D0%B5%D1%82%D1%80%D0%B8">сети Петри</a>

Базовая сеть Петри - граф, состоящий из чередующихся узлов и переходов. В каждой вершине может содержаться от 0 до бесконечности фишек.
Переход возможен, если у всех входных узлов есть достаточное количество фишек. Переход считается атомарной операцией.

С помощью сети Петри можно симулировать другие вещи, такие как:
- всякие примитивы синхронизации - <a href="https://github.com/alex-ak1/petry/wiki/petry1">семафоры, мьютексы</a> и так далее.
- логические элементы - все булевы операции.

# организация сети
Сеть состоит из следующих частей:
- список узлов. содержать фишки.
- список переходов. фишки не содержат, но описывают откуда и куда они идут.
-- входные и выходные связи. Каждый переход имеет несколько входных связей и выходных (несколько это в том числе 0).

Для визуализации можно добавить во все эти элементы различные украшения - цветные фишки (может быть полезно и для визуализации, и для логики), цветные узлы и переходы.


