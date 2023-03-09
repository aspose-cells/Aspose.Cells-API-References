---
title: get_values метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 30
url: /ru/python-net/aspose.cells/referredarea/get_values/
is_root: false
---
##  get_values() {#}
Получает значения ячеек в этой области.


###  Возвращает

Если эта область недействительна, будет возвращено "#REF!";
Если эта область представляет собой одну ячейку, верните объект значения ячейки;
В противном случае верните один 2D-массив для всех значений в этой области.


```python
def get_values(self):
    ...
```




##  get_values(calculate_formulas) {#bool}
Получает значения ячеек в этой области.


###  Возвращает

Если эта область недействительна, будет возвращено "#REF!";
Если эта область представляет собой одну ячейку, верните объект значения ячейки;
В противном случае верните один 2D-массив для всех значений в этой области.


```python
def get_values(self, calculate_formulas):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| calculate_formulas | bool | В этом диапазоне, если есть какие-то формулы, которые не были рассчитаны,<br/> этот флаг указывает, должны ли эти формулы вычисляться рекурсивно|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [ReferredArea](/cells/ru/python-net/aspose.cells/referredarea)
