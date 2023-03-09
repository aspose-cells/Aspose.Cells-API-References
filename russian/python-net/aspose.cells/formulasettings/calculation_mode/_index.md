---
title: calculation_mode недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 60
url: /ru/python-net/aspose.cells/formulasettings/calculation_mode/
is_root: false
---
##  calculation_mode недвижимость

Получает или задает режим расчета рабочей книги в MS Excel.

###  Примечания

Это свойство предназначено только для сохранения настроек в результирующий файл электронной таблицы.
чтобы другие приложения (например, MS Excel) могли действовать соответствующим образом при загрузке и манипулировании результирующим файлом.
Из соображений производительности для большинства пользовательских приложений мы не вычисляем никакие формулы в рабочей книге автоматически,
независимо от того, какой режим был установлен для этого свойства.
Если пользователю необходимо вычислить формулы, всегда вызывайте методы для разных объектов в соответствии с требованиями:
[Workbook.calculate_formula()](/cells/python-net/aspose.cells/workbook/calculate_formula), [Worksheet.calculate_formula(formula)](/cells/python-net/aspose.cells/worksheet/calculate_formula),
[Cell.calculate(options)](/cells/ru/python-net/aspose.cells/cell/calculate), ...и т.д.
###  Определение:
```python
@property
def calculation_mode(self):
    ...
@calculation_mode.setter
def calculation_mode(self, value):
    ...
```

###  Смотрите также
* модуль [aspose.cells](../../)
* класс [CalcModeType](/cells/ru/python-net/aspose.cells/calcmodetype)
* класс [FormulaSettings](/cells/ru/python-net/aspose.cells/formulasettings)
