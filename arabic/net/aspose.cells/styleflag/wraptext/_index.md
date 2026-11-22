---
title: "StyleFlag.WrapText"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية StyleFlag. سيتم تطبيق إعداد التفاف النص"
type: docs
url: /ar/net/aspose.cells/styleflag/wraptext/
---
## StyleFlag.WrapText property

سيتم تطبيق إعداد التفاف النص.

```csharp
public bool WrapText { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StyleFlagPropertyWrapTextDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نمط مع تمكين التفاف النص
            Style style = workbook.CreateStyle();
            style.IsTextWrapped = true;

            // إنشاء علم نمط وتمكين علم WrapText
            StyleFlag flag = new StyleFlag();
            flag.WrapText = true;

            // تطبيق النمط على الخلية A1 مع الأعلام المحددة
            worksheet.Cells["A1"].PutValue("This is a long text that should wrap in the cell");
            worksheet.Cells.ApplyStyle(style, flag);

            // ضبط ارتفاع الصف تلقائيًا لرؤية النص الملتف
            worksheet.AutoFitRow(0);

            // احفظ المصنف
            workbook.Save("WrapTextDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


