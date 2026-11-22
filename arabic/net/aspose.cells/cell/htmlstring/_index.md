---
title: "Cell.HtmlString"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Cell. تحصل وتعيّن سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذه الخلية"
type: docs
url: /ar/net/aspose.cells/cell/htmlstring/
---
## Cell.HtmlString property

يحصل على سلسلة HTML أو يضبطها التي تحتوي على بيانات وبعض التنسيقات في هذه الخلية.

```csharp
public string HtmlString { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyHtmlStringDemo
    {
        public static void Run()
        {
            // إنشاء كائن دفتر عمل
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى مجموعة الخلايا
            Cells cells = worksheet.Cells;
            
            // تعيين سلسلة HTML مع التنسيق إلى الخلية A1
            cells["A1"].HtmlString = "This is <b>bold</b> and <i>italic</i> text<br>with a line break";
            
            // احفظ المصنف
            workbook.Save("HtmlStringDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


