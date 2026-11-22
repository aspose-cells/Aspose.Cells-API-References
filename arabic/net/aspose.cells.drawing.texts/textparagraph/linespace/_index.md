---
title: "TextParagraph.LineSpace"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextParagraph. تحصل أو تعين مقدار المسافة الرأسية البيضاء التي ستُستخدم داخل الفقرة"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textparagraph/linespace/
---
## TextParagraph.LineSpace property

الحصول وتعيين مقدار المسافة البيضاء العمودية التي سيتم استخدامها داخل الفقرة.

```csharp
public double LineSpace { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextParagraphPropertyLineSpaceDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة شكل مربع نص
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            shape.Text = "First line\nSecond line";
            
            // الوصول إلى فقرات النص
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // تكوين تباعد الأسطر للفقرة الثانية
            TextParagraph paragraph = paragraphs[1];
            paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            paragraph.LineSpace = 2; // Set line spacing to 2 points
            
            // احفظ وأعد التحميل لإظهار الاستمرارية
            string outputPath = "output_LineSpaceDemo.xlsx";
            workbook.Save(outputPath);
            
            // إعادة التحميل للتحقق من الإعدادات
            Workbook loadedWorkbook = new Workbook(outputPath);
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            TextParagraph loadedParagraph = loadedShape.TextBody.TextParagraphs[1];
            
            Console.WriteLine("Line space: " + loadedParagraph.LineSpace);
            Console.WriteLine("Line space type: " + loadedParagraph.LineSpaceSizeType);
        }
    }
}
```

### انظر أيضًا

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


