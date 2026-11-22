---
title: "TextParagraph.LeftMargin"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextParagraph. تحدد الهامش الأيسر للفقرة"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textparagraph/leftmargin/
---
## TextParagraph.LeftMargin property

يحدد الهامش الأيسر للفقرة.

```csharp
public double LeftMargin { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyLeftMarginDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مربع نص إلى ورقة العمل
            TextBox textBox = worksheet.Shapes.AddTextBox(0, 0, 2, 2, 200, 200);
            textBox.Text = "This is a sample text paragraph.\nSecond line of the paragraph.";

            // الحصول على فقرة النص من الفقرة الأولى لمربع النص
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // اعرض قيمة الهامش الأيسر الحالية
            Console.WriteLine("Current LeftMargin value: " + paragraph.LeftMargin);

            // عيّن قيمة جديدة للهامش الأيسر (بالنقاط)
            paragraph.LeftMargin = 20.0;

            // أظهر التأثير بإضافة مربع نص آخر بهامش افتراضي
            TextBox textBox2 = worksheet.Shapes.AddTextBox(0, 3, 2, 2, 200, 200);
            textBox2.Text = "This text box has default left margin.\nCompare the indentation.";

            // احفظ المصنف لإظهار الفرق
            workbook.Save("TextParagraphLeftMarginDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


