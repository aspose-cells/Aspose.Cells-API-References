---
title: "PivotField.Ungroup"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة PivotField. إلغاء تجميع حقل المحور"
type: docs
url: /ar/net/aspose.cells.pivot/pivotfield/ungroup/
---
## PivotField.Ungroup method

إلغاء تجميع الحقل المحوري.

```csharp
public void Ungroup()
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldMethodUngroupDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("example.xlsx");
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى أول جدول محوري
            PivotTable pivotTable = worksheet.PivotTables[0];
            
            // إلغاء تجميع حقل العمود الأول
            pivotTable.ColumnFields[0].Ungroup();
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


