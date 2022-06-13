---
title: CalculatedValue
second_title: Справочник по Aspose.Cells для .NET API
description: Получает или задает вычисленное значение для этой функции.
type: docs
weight: 10
url: /ru/net/aspose.cells/calculationdata/calculatedvalue/
---
## CalculationData.CalculatedValue property

Получает или задает вычисленное значение для этой функции.

```csharp
public object CalculatedValue { get; set; }
```

### Примечания

Пользователь должен установить это свойство в своем пользовательском механизме расчета для тех функций, которые поддерживает механизм, и набор значение будет возвращено при получении этого свойства позже. Установленное значение может быть любым значением тех объектов, которые могут быть установлены в Cell(Cell.Value). А также это может быть массив таких значений, или Range, Name, ReferredArea. Получение этого свойства перед настройкой приведет к тому, что функция будет вычислена механизмом расчета Aspose.Cells по умолчанию, и вычисленное значение будет возвращено.

### Смотрите также

* class [CalculationData](../../calculationdata)
* пространство имен [Aspose.Cells](../../calculationdata)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->