---
title: "PivotFieldGroupOptions.GroupType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية PivotFieldGroupOptions. تحصل أو تعين نوع التجميع لحقل المحور. فقط لتجميع حقل محور التاريخ والوقت"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfieldgroupoptions/grouptype/
---
## PivotFieldGroupOptions.GroupType property

يحصل أو يضبط نوع التجميع لحقل المحور. فقط لتجميع حقل المحور الزمني.

```csharp
public PivotGroupByType GroupType { get; set; }
```

### أمثلة

```csharp
//init
PivotFieldGroupOptions pivotFieldGroupOptions = new PivotFieldGroupOptions();
// تجميع حسب السنة والشهر معًا
PivotGroupByType pivotGroupByType = pivotFieldGroupOptions.GroupType;
pivotGroupByType = PivotGroupByType.Years | PivotGroupByType.Months;
pivotFieldGroupOptions.GroupType = pivotGroupByType;
```

### انظر أيضًا

* enum [PivotGroupByType](../../pivotgroupbytype/)
* class [PivotFieldGroupOptions](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


