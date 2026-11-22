---
title: "ValidationCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ValidationCollection. تضيف تحققًا من البيانات إلى المجموعة"
type: docs
url: /ar/net/aspose.cells/validationcollection/add/
---
## Add() {#add}

يضيف تحققًا من البيانات إلى المجموعة.

```csharp
[Obsolete("Use ValidationCollection.Add(CellArea) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add()
```

### قيمة الإرجاع

[`Validation`](../../validation/) object index.

### ملاحظات

ملاحظة: هذه الطريقة الآن مهجورة. بدلاً من ذلك، يرجى استخدام طريقة ValidationCollection.Add(CellArea). سيتم إزالة هذه الطريقة بعد 12 شهرًا منذ JANUARY 2015. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### انظر أيضًا

* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## Add(CellArea) {#add_1}

يضيف تحققًا من البيانات إلى المجموعة.

```csharp
public int Add(CellArea ca)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| ca | CellArea | المنطقة تحتوي على هذا التحقق. |

### قيمة الإرجاع

[`Validation`](../../validation/) object index.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ValidationCollectionMethodAddWithCellAreaDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // إنشاء منطقة خلية للتحقق
            CellArea cellarea = new CellArea();
            cellarea.StartRow = 0;
            cellarea.StartColumn = 0;
            cellarea.EndRow = 1;
            cellarea.EndColumn = 1;
            
            // إضافة التحقق إلى المجموعة
            int index = sheet.Validations.Add(cellarea);
            Validation validation = sheet.Validations[index];
            
            // تكوين إعدادات التحقق
            validation.Type = ValidationType.List;
            validation.Formula1 = "Yes,No";
            validation.AlertStyle = ValidationAlertType.Information;
            
            // احفظ المصنف
            workbook.Save("ValidationCollectionMethodAddWithCellAreaDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


