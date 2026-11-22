---
title: "TextParagraph.SpaceBefore"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextParagraph. تحصل وتضبط مقدار المسافة العمودية الفارغة التي ستكون موجودة قبل الفقرة"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textparagraph/spacebefore/
---
## TextParagraph.SpaceBefore property

يحصل على ويضبط مقدار المسافة الرأسية الفارغة التي ستكون موجودة قبل الفقرة.

```csharp
public double SpaceBefore { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertySpaceBeforeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف مربع نص وحدد النص
            Aspose.Cells.Drawing.Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First paragraph\nSecond paragraph";
            
            // احصل على الفقرات
            Aspose.Cells.Drawing.Texts.TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // اضبط تباعد الفقرة الثانية
            Aspose.Cells.Drawing.Texts.TextParagraph p = paragraphs[1];
            p.LineSpaceSizeType = Aspose.Cells.Drawing.Texts.LineSpaceSizeType.Points;
            p.LineSpace = 2;
            p.SpaceAfter = 3;
            p.SpaceBefore = 4; // Demonstrate SpaceBefore property
            
            // حفظ والتحقق
            string outputPath = "output_SpaceBeforeDemo.xlsx";
            workbook.Save(outputPath);
            
            Console.WriteLine("Demo completed. File saved: " + outputPath);
        }
    }
}
```

### انظر أيضًا

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


