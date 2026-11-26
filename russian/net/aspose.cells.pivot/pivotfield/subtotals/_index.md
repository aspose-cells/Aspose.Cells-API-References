---
title: "PivotField.Subtotals"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство PivotField. Получает или задает промежуточные итоги поля. Только для строкового или столбцового поля сводки"
type: docs
url: /ru/net/aspose.cells.pivot/pivotfield/subtotals/
---
## PivotField.Subtotals property

Получает или задает промежуточные итоги поля. Только для строкового или столбцового сводного поля.

```csharp
public PivotFieldSubtotalType Subtotals { get; set; }
```

### Примеры

```csharp

[C#]
//Без промежуточных итогов
rowField.Subtotals = PivotFieldSubtotalType.None;
//Автоматические промежуточные итоги
//rowField.Subtotals = PivotFieldSubtotalType.Automatic;
//Одинарные итоги: Sum
//rowField.Subtotals = PivotFieldSubtotalType.Sum;
//Множественные итоги: Sum и count numbers 
//rowField.Subtotals = PivotFieldSubtotalType.Sum | PivotFieldSubtotalType.Count;
```

### См. также

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


