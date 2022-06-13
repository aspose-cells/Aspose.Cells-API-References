---
title: EnableCalculationChain
second_title: Справочник по Aspose.Cells для .NET API
description: Включить ли цепочку вычислений для формул. Значение по умолчанию  ложь.
type: docs
weight: 50
url: /ru/net/aspose.cells/formulasettings/enablecalculationchain/
---
## FormulaSettings.EnableCalculationChain property

Включить ли цепочку вычислений для формул. Значение по умолчанию — ложь.

```csharp
public bool EnableCalculationChain { get; set; }
```

### Примечания

Когда в рабочей книге много формул и пользователю нужно вычислить их несколько раз с изменением лишь небольшой их части может быть полезно для производительности включить цепочку вычислений. С другой стороны, если цепочка включена, поддержание модели цепочки требует дополнительной памяти, и также требует немного больше процессорного времени для некоторых других операций, таких как изменение значение ячейки или формулы. После изменения этого свойства с false на true цепочка вычислений будет проанализирована и построена во время первого вычисления для рабочей книги, поэтому необходимое время для первого вычисления может быть больше, чем обычный расчет без цепочки.

### Смотрите также

* class [FormulaSettings](../../formulasettings)
* пространство имен [Aspose.Cells](../../formulasettings)
* сборка [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->