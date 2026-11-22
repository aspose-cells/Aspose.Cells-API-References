---
title: "Range.EntireColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Range. يحصل على كائن Range يمثل العمود بالكامل أو الأعمدة التي تحتوي على النطاق المحدد"
type: docs
url: /ar/net/aspose.cells/range/entirecolumn/
---
## Range.EntireColumn property

يحصل على كائن Range يمثل العمود بالكامل (أو الأعمدة) الذي يحتوي على النطاق المحدد.

```csharp
public Range EntireColumn { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyEntireColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء نطاق يبدأ من الخلية C1 (الصف 0، العمود 2)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange(0, 2, 1, 1);
            
            // احصل على العمود بالكامل الذي يحتوي على النطاق (العمود C)
            Aspose.Cells.Range entireColumn = range.EntireColumn;
            
            // تطبيق التنسيق على العمود بالكامل
            Style style = entireColumn[0, 0].GetStyle();
            style.Custom = "##0%";
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.NumberFormat = true;
            entireColumn.ApplyStyle(style, styleFlag);
            
            // احفظ المصنف
            workbook.Save("EntireColumnDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


