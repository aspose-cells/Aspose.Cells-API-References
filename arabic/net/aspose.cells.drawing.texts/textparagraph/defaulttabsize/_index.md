---
title: "TextParagraph.DefaultTabSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextParagraph. تحصل وتعيّن الحجم الافتراضي لحرف التبويب داخل هذه الفقرة"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textparagraph/defaulttabsize/
---
## TextParagraph.DefaultTabSize property

الحصول وتعيين الحجم الافتراضي لحرف الجدولة داخل هذه الفقرة.

```csharp
public double DefaultTabSize { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyDefaultTabSizeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مربع نص إلى ورقة العمل
            TextBox textBox = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 300, 200);
            textBox.Text = "Item\tPrice\tQuantity\nPen\t$1.20\t10\nNotebook\t$2.50\t5";

            // الحصول على فقرة النص من الفقرة الأولى لمربع النص
            TextParagraph paragraph = textBox.TextBody.TextParagraphs[0];

            // عرض الحجم الافتراضي الحالي للتبويب
            Console.WriteLine("Current DefaultTabSize: " + paragraph.DefaultTabSize);

            // عيّن حجم تبويب أصغر (الإعداد الافتراضي عادةً حوالي 36 نقطة)
            paragraph.DefaultTabSize = 20.0;
            Console.WriteLine("DefaultTabSize set to: " + paragraph.DefaultTabSize);

            // أضف مربع نص آخر بحجم تبويب افتراضي للمقارنة
            TextBox textBox2 = worksheet.Shapes.AddTextBox(1, 3, 1, 3, 300, 200);
            textBox2.Text = "Item\tPrice\tQuantity\nPen\t$1.20\t10\nNotebook\t$2.50\t5";

            // احفظ المصنف لرؤية الفرق في تباعد التبويبات
            workbook.Save("TextParagraphDefaultTabSizeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


