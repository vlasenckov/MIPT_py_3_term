#  Принцип инверчсии зависимостей
------
Приблизительно оригинальная формулировка такова:
- Модули верхних уровней не должны зависеть от модулей нижних уровней. Оба типа модулей должны зависеть от абстракций.
- Абстракции не должны зависеть от деталей. Детали должны зависеть от абстракций.

Другими словами, требуется, чтобы отдeльно взятые модули связывались друг с другом не напрямую, а через некоторые абстракции, например, интерфейсы или абстрактные классы. Таким образом, мы уменьшим связность модулей, в плане того, что теперь моудль верхнего уровня даже не знает о том, какой именно модуль  нижнего уровня с ним контактирует, так как теперь в его поле зрения некоторая абстракция. 
Второе же утверждение крайне логичное и скорее даже ссылает нас на открытость-заркрытость: опять же некоторый интерфейс должен быть открытым к добавлению новых версий деталей, а это возможно только при соблюдении второго утверждения.