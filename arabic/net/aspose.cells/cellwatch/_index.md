---
title: "الفئة CellWatch"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.CellWatch. تمثل عنصر مراقبة الخلية في نافذة المراقبة"
type: docs
url: /ar/net/aspose.cells/cellwatch/
---
## CellWatch class

يمثل عنصر مراقبة الخلية في 'نافذة المراقبة'.

```csharp
public class CellWatch
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [CellWatch](cellwatch/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CellName](../../aspose.cells/cellwatch/cellname/) { get; set; } | يحصل على اسم الخلية ويضبطه. |
| [Column](../../aspose.cells/cellwatch/column/) { get; set; } | يحصل على عمود الخلية ويضبطه. |
| [Row](../../aspose.cells/cellwatch/row/) { get; set; } | يحصل على صف الخلية ويضبطه. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellWatchDemo
    {
        public static void CellWatchExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            // احصل على ورقة العمل الأولى.
            Worksheet sheet = workbook.Worksheets[0];

            // أضف عنصر مراقبة الخلية إلى نافذة المراقبة
            int watchIndex = sheet.CellWatches.Add("B2");

            // استرجع كائن CellWatch
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // ضبط الخصائص
            cellWatch.Row = 1; // B2 corresponds to row 1 (0-based index)
            cellWatch.Column = 1; // B2 corresponds to column 1 (0-based index)
            cellWatch.CellName = "B2";

            // احفظ المصنف
            workbook.Save("CellWatchExample.xlsx");
            workbook.Save("CellWatchExample.pdf");
            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


