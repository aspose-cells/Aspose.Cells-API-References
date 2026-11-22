---
title: "PivotField.Subtotals"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotField. يحصل أو يحدد المجاميع الفرعية للحقل. فقط لحقل الصف أو العمود"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/subtotals/
---
## PivotField.Subtotals property

يحصل أو يعيّن المجاميع الفرعية للحقل. فقط لحقل المحور الصف أو العمود.

```csharp
public PivotFieldSubtotalType Subtotals { get; set; }
```

### أمثلة

```csharp

[C#]
//بدون مجاميع فرعية
rowField.Subtotals = PivotFieldSubtotalType.None;
//مجاميع فرعية تلقائية
//rowField.Subtotals = PivotFieldSubtotalType.Automatic;
//مجاميع فرعية فردية: Sum
//rowField.Subtotals = PivotFieldSubtotalType.Sum;
//مجاميع فرعية متعددة: Sum و count numbers
//rowField.Subtotals = PivotFieldSubtotalType.Sum | PivotFieldSubtotalType.Count;
```

### انظر أيضًا

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


