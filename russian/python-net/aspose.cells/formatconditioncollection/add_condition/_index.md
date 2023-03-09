---
title: add_condition метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 40
url: /ru/python-net/aspose.cells/formatconditioncollection/add_condition/
is_root: false
---
##  add_condition(type) {#FormatConditionType}
Добавьте условие формата.


###  Возвращает

Индекс объекта условия форматирования;


```python
def add_condition(self, type):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| type | [FormatConditionType](/cells/ru/python-net/aspose.cells/formatconditiontype) | Тип условия формата.|


##  add_condition(type, operator_type, formula1, formula2) {#FormatConditionType-OperatorType-str-str}
Добавляет условие форматирования.


###  Возвращает

Индекс объекта условия форматирования;


```python
def add_condition(self, type, operator_type, formula1, formula2):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| type | [FormatConditionType](/cells/ru/python-net/aspose.cells/formatconditiontype) | [FormatConditionType](/cells/ru/python-net/aspose.cells/formatconditiontype) условного форматирования.<br/> Это может быть один из членов FormatConditionType.|
| operator_type | [OperatorType](/cells/ru/python-net/aspose.cells/operatortype) | Сравнение [OperatorType](/cells/ru/python-net/aspose.cells/operatortype).<br/> Это может быть один из членов OperatorType.|
| formula1 | str |Значение или выражение, связанное с условным форматированием.<br/>Если входное значение начинается с '=', то оно будет принято как формула.<br/>В противном случае оно будет принято как простое значение (текст, число, логическое значение).<br/> Для текстового значения, которое начинается с '=', пользователь может ввести его как формулу в формате: "=\"=...\"".|
| formula2 | str |Значение или выражение, связанное с условным форматированием.<br/> Формат ввода такой же, как и в формуле1|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [FormatConditionCollection](/cells/ru/python-net/aspose.cells/formatconditioncollection)
* класс [FormatConditionType](/cells/ru/python-net/aspose.cells/formatconditiontype)
* класс [OperatorType](/cells/ru/python-net/aspose.cells/operatortype)
