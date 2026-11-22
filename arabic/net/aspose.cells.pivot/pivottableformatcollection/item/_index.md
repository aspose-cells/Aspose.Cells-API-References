---
title: "PivotTableFormatCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "PivotTableFormatCollection خاصية. يحصل على التنسيق حسب الفهرس"
type: docs
url: /ar/net/aspose.cells.pivot/pivottableformatcollection/item/
---
## PivotTableFormatCollection indexer

يحصل على التنسيق حسب الفهرس.

```csharp
public PivotTableFormat this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableFormatCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // إنشاء مصنف من ملف Excel المصدر
            Workbook workbook = new Workbook("example.xlsx");

            // تحديث جميع جداول المحور
            workbook.Worksheets.RefreshAll();
            Cells cells = workbook.Worksheets[0].Cells;

            // الوصول إلى أول جدول محوري
            PivotTable pt = workbook.Worksheets[0].PivotTables[0];

            // عرض خاصية Item عن طريق الوصول إلى أول PivotFormat
            pt.PivotFormats[0].PivotArea.OnlyData = false;
            workbook.Worksheets.RefreshAll();

            // تغيير إعدادات التنسيق باستخدام خاصية Item
            pt.PivotFormats[0].PivotArea.OnlyLabel = true;
            workbook.Worksheets.RefreshAll();

            // احفظ المصنف المعدل
            workbook.Save("modified_example.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [PivotTableFormat](../../pivottableformat/)
* class [PivotTableFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


