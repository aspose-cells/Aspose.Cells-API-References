---
title: "MsoLineFormat.ForeColor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية MsoLineFormat. تحصل وتضبط لون الخط الأمامي للحد"
type: docs
url: /ar/net/aspose.cells.drawing/msolineformat/forecolor/
---
## MsoLineFormat.ForeColor property

يحصل على ويضبط لون مقدمة خط الحدود.

```csharp
public Color ForeColor { get; set; }
```

### أمثلة

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyForeColorDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 200, 100);
            
            // تعيين خصائص تنسيق الخط بما في ذلك ForeColor
            textBox.LineFormat.ForeColor = Color.Red;
            textBox.LineFormat.Style = MsoLineStyle.Single;
            textBox.LineFormat.IsVisible = true;
            textBox.LineFormat.Weight = 2;

            workbook.Save("MsoLineFormatForeColorDemo.xlsx", SaveFormat.Xlsx);
            
            // تحقق من اللون المحفوظ
            Workbook loadedWorkbook = new Workbook("MsoLineFormatForeColorDemo.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            Console.WriteLine("Line ForeColor: " + loadedShape.LineFormat.ForeColor.ToString());
        }
    }
}
```

### انظر أيضًا

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


