---
title: "Style.Name"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Style. تحصل أو تعين اسم النمط"
type: docs
url: /ar/net/aspose.cells/style/name/
---
## Style.Name property

يحصل على اسم النمط أو يضبطه.

```csharp
public string Name { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class StylePropertyNameDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إنشاء وتطبيق النمط المسمى الأول
            Style style1 = workbook.CreateStyle();
            style1.Number = 7;
            style1.Name = "Sales";
            worksheet.Cells["A1"].SetStyle(style1);
            worksheet.Cells["A1"].PutValue("Sales Data");
            
            // إنشاء وتطبيق النمط المسمى الثاني
            Style style2 = workbook.CreateStyle();
            style2.Font.Size = 14;
            style2.Font.IsBold = true;
            style2.Font.IsItalic = true;
            style2.Font.Color = System.Drawing.Color.Yellow;
            style2.ForegroundColor = System.Drawing.Color.Blue;
            style2.Pattern = BackgroundType.Solid;
            style2.Name = "Header";
            worksheet.Cells["B1"].SetStyle(style2);
            worksheet.Cells["B1"].PutValue("Header Text");
            
            // احفظ المصنف
            workbook.Save("StylePropertyNameDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


