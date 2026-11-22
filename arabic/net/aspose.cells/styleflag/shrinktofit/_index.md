---
title: "StyleFlag.ShrinkToFit"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق إعداد التقليص لتناسب"
type: docs
url: /ar/net/aspose.cells/styleflag/shrinktofit/
---
## StyleFlag.ShrinkToFit property

سيتم تطبيق إعداد التصغير لتناسب.

```csharp
public bool ShrinkToFit { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyShrinkToFitDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين بيانات عينة في خلية
            cells["A1"].PutValue("This is a long text that needs to fit in the cell");
            
            // إنشاء نمط مع تمكين ShrinkToFit
            Style style = workbook.CreateStyle();
            style.ShrinkToFit = true;
            
            // إنشاء علم نمط وتمكين علم ShrinkToFit
            StyleFlag flag = new StyleFlag();
            flag.ShrinkToFit = true;
            
            // تطبيق النمط على نطاق الخلايا (باستخدام Aspose.Cells.Range صراحةً)
            Aspose.Cells.Range range = cells.CreateRange("A1");
            range.ApplyStyle(style, flag);
            
            // تعيين عرض العمود لتوضيح التقليص
            worksheet.Cells.SetColumnWidth(0, 10);
            
            // احفظ المصنف
            workbook.Save("ShrinkToFitDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


