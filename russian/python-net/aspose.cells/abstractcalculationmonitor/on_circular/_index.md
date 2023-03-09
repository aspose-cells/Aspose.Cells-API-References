---
title: on_circular метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 40
url: /ru/python-net/aspose.cells/abstractcalculationmonitor/on_circular/
is_root: false
---
##  on_circular(circular_cells_data) {#collections.abc.Iterator}
Реализуйте этот метод для ведения бизнеса при расчете формул с циклическими ссылками.


###  Возвращает

Нужно ли обработчику формул вычислять эти ячейки по кругу после этого вызова.
Значение true, чтобы обработчик формул продолжал выполнять для них расчеты.
False, чтобы обработчик формул просто помечал эти ячейки как рассчитанные.


```python
def on_circular(self, circular_cells_data):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| circular_cells_data | collections.abc.Iterator | IEnumerator с элементами CalculationCell, представляющими ячейки, которые<br/> зависят от циклических ссылок.|
###  Примечания

В реализации пользователь также может установить ожидаемое значение как вычисленный результат.
для части/всех этих ячеек, чтобы механизм формул не вычислял их рекурсивно.


###  Смотрите также
* модуль [aspose.cells](../../)
* класс [AbstractCalculationMonitor](/cells/ru/python-net/aspose.cells/abstractcalculationmonitor)
