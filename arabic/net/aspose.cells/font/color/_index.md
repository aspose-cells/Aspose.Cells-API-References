---
title: "Font.Color"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Font. تحصل أو تضبط لون الخط"
type: docs
url: /ar/net/aspose.cells/font/color/
---
## Font.Color property

يحصل أو يضبط لون الخط.

```csharp
public Color Color { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class FontPropertyColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين HTML بألوان خطوط مختلفة وأنماط
            Cell cell = worksheet.Cells["A1"];
            cell.HtmlString = "<font color='Red'>Red Text</font> <font color='#0000FF'>Blue Text</font><font style='color:#00FF00;text-decoration: underline;'>Green Underlined</font>";
            
            // الحصول على تنسيق النص الغني
            FontSetting[] richText = cell.GetCharacters();
            
            // التحقق وعرض خصائص اللون
            Console.WriteLine("First segment color: " + richText[0].Font.Color);
            Console.WriteLine("Second segment color: " + richText[1].Font.Color);
            Console.WriteLine("Third segment underline: " + richText[2].Font.Underline);
            
            // احفظ المصنف
            workbook.Save("FontColorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


