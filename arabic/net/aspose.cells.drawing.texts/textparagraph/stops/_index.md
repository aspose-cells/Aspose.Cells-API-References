---
title: "TextParagraph.Stops"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextParagraph. تحصل على قائمة نقاط التبويب"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textparagraph/stops/
---
## TextParagraph.Stops property

يحصل على قائمة نقاط التبويب.

```csharp
public TextTabStopCollection Stops { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextParagraphPropertyStopsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف نصاً إلى خلية واحصل على خصائص فقرة النص الخاصة بها
            worksheet.Cells["A1"].PutValue("Sample\tText\tWith\tTabs");
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 200, 200);
            shape.Text = "Sample\tText\tWith\tTabs";
            
            // احصل على فقرة النص
            var textOptions = shape.TextBody.TextParagraphs[0];

            // اعرض عدد نقاط التبويب الحالية
            Console.WriteLine("Current tab stops count: " + textOptions.Stops.Count);

            // أضف نقاط تبويب جديدة
            textOptions.Stops.Add(TextTabAlignmentType.Left, 50);
            textOptions.Stops.Add(TextTabAlignmentType.Center, 100);
            textOptions.Stops.Add(TextTabAlignmentType.Right, 150);

            // عرض مسافات التبويب المحدثة
            Console.WriteLine("Updated tab stops count: " + textOptions.Stops.Count);
            for (int i = 0; i < textOptions.Stops.Count; i++)
            {
                Console.WriteLine($"Tab {i+1}: Position={textOptions.Stops[i].TabPosition}, Alignment={textOptions.Stops[i].TabAlignment}");
            }

            // حفظ المصنف لرؤية التأثير
            workbook.Save("TextParagraphStopsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextTabStopCollection](../../texttabstopcollection/)
* class [TextParagraph](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


