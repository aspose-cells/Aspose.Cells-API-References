---
title: set_formulas метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 60
url: /ru/python-net/aspose.cells/formatcondition/set_formulas/
is_root: false
---
##  set_formulas(formula1, formula2, is_r1c1, is_local) {#str-str-bool-bool}
Задает значение или выражение, связанное с этим условием формата.



```python
def set_formulas(self, formula1, formula2, is_r1c1, is_local):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| formula1 | str | Значение или выражение, связанное с этим условием формата.<br/>Если входное значение начинается с '=', то оно будет принято как формула. В противном случае оно будет принято как простое значение (текст, число, логическое значение).<br/> Для текстового значения, которое начинается с '=', пользователь может ввести его как формулу в формате: "=\"=...\"".|
| formula2 | str | Значение или выражение, связанное с этим условием формата. Формат ввода такой же, как и в формуле1|
| is_r1c1 | bool | Является ли формула формулой R1C1.|
| is_local | bool | Отформатирована ли формула в языковом стандарте.|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [FormatCondition](/cells/ru/python-net/aspose.cells/formatcondition)
