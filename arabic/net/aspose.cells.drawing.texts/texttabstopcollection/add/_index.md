---
title: "TextTabStopCollection.Add"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة TextTabStopCollection. تُضيف علامة تبويب"
type: docs
url: /ar/net/aspose.cells.drawing.texts/texttabstopcollection/add/
---
## TextTabStopCollection.Add method

يضيف نقطة تبويب.

```csharp
public int Add(TextTabAlignmentType tabAlignment, double tabPosition)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| tabAlignment | TextTabAlignmentType |  |
| tabPosition | Double |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextTabStopCollectionMethodAddWithTextTabAlignmentTypeDoubleDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء شكل لإضافة نص مع علامات تبويب
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 100, 200);
            var textParagraph = shape.TextBody.TextParagraphs[0];
            
            // احصل على TextTabStopCollection
            var tabStops = textParagraph.Stops;

            try
            {
                // استدعِ طريقة Add مع TextTabAlignmentType.Left والموضع 50.0
                int index1 = tabStops.Add(TextTabAlignmentType.Left, 50.0);
                
                // استدعِ طريقة Add مع TextTabAlignmentType.Right والموضع 100.0
                int index2 = tabStops.Add(TextTabAlignmentType.Right, 100.0);
                
                // أضف نصًا مع علامات تبويب لتوضيح علامات التبويب
                shape.Text = "Left-aligned\tRight-aligned";

                Console.WriteLine("Added tab stops at positions 50.0 (Left) and 100.0 (Right)");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
            
            // حفظ النتيجة
            workbook.Save("TextTabStopCollectionMethodAddDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [TextTabAlignmentType](../../texttabalignmenttype/)
* class [TextTabStopCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


