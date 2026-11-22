---
title: "FileFontSource.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FileFontSource. تُرجع نوع مصدر الخط"
type: docs
url: /ar/net/aspose.cells/filefontsource/type/
---
## FileFontSource.Type property

يرجع نوع مصدر الخط.

```csharp
public override FontSourceType Type { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FileFontSourcePropertyTypeDemo
    {
        public static void Run()
        {
            string fontFilePath = "CustomFont.ttf";
            
            // إنشاء كائن FileFontSource
            FileFontSource fontSource = new FileFontSource(fontFilePath);
            
            // توضيح استخدام خاصية Type
            Console.WriteLine("Font Source Type: " + fontSource.Type);
            
            // إنشاء دفتر عمل وتطبيق الخط
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            Cell cell = sheet.Cells["A1"];
            cell.PutValue("Text with custom font");
            
            Style style = cell.GetStyle();
            style.Font.Name = "CustomFont";
            cell.SetStyle(style);
            
            workbook.Save("FontSourceDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [FontSourceType](../../fontsourcetype/)
* class [FileFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


