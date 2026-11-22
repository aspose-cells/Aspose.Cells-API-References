---
title: "TextOptions.FarEastName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextOptions. تحصل وتعيّن اسم FarEast"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textoptions/fareastname/
---
## TextOptions.FarEastName property

يحصل على اسم FarEast ويضبطه.

```csharp
public string FarEastName { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextOptionsPropertyFarEastNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكلاً واضبط خط FarEastName
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            shape.Text = "Sample Text";
            shape.TextOptions.FarEastName = "宋体";

            // احفظ وأعد التحميل للتحقق
            string outputPath = "output_FarEastName.xlsx";
            workbook.Save(outputPath);

            // أعد التحميل للتحقق
            Workbook verifyWorkbook = new Workbook(outputPath);
            Aspose.Cells.Drawing.Shape verifyShape = verifyWorkbook.Worksheets[0].Shapes[0];
            Console.WriteLine("FarEastName: " + verifyShape.TextOptions.FarEastName);
        }
    }
}
```

### انظر أيضًا

* class [TextOptions](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


