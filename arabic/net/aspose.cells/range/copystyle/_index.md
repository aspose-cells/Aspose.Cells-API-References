---
title: "Range.CopyStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. ينسخ إعدادات النمط من نطاق مصدر"
type: docs
url: /ar/net/aspose.cells/range/copystyle/
---
## Range.CopyStyle method

ينسخ إعدادات النمط من نطاق مصدر.

```csharp
public void CopyStyle(Range range)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| range | Range | كائن المصدر [`Range`](../). |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodCopyStyleWithRangeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet sheetSrc = workbook.Worksheets[0];
            sheetSrc.Name = "Source";
            
            // أضف بعض النمط النموذجي إلى النطاق المصدر
            Cells cellsSrc = sheetSrc.Cells;
            Aspose.Cells.Range rangeSrc = cellsSrc.CreateRange("A1:D5");
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 14;
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;
            rangeSrc.SetStyle(style);
            
            // إنشاء ورقة عمل الوجهة
            Worksheet sheetDest = workbook.Worksheets[workbook.Worksheets.Add()];
            sheetDest.Name = "Destination";
            
            // إنشاء نطاق الوجهة ونسخ النمط
            Cells cellsDest = sheetDest.Cells;
            Aspose.Cells.Range rangeDest = cellsDest.CreateRange("A1:D5");
            rangeDest.CopyStyle(rangeSrc);
            
            // احفظ المصنف
            workbook.Save("RangeCopyStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


