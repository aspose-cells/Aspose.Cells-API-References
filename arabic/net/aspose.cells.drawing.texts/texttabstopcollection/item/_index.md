---
title: "TextTabStopCollection.Item"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية TextTabStopCollection. تُرجع TextTabStop حسب الفهرس"
type: docs
url: /ar/net/aspose.cells.drawing.texts/texttabstopcollection/item/
---
## TextTabStopCollection indexer

يُرجع [`TextTabStop`](../../texttabstop/) حسب الفهرس.

```csharp
public TextTabStop this[int index] { get; }
```

| معامل | الوصف |
| --- | --- |
| فهرس | الفهرس. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextTabStopCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا جديدًا واحصل على ورقة العمل الأولى
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف شكل صندوق نص يحتوي على أحرف تبويب
            var shape = worksheet.Shapes.AddTextBox(1, 0, 1, 0, 300, 50);
            shape.Text = "Left\tCenter\tRight";

            // الوصول إلى مجموعة علامات تبويب الفقرة الأولى
            var textParagraph = shape.TextBody.TextParagraphs[0];
            var tabStops = textParagraph.Stops;

            // تحضير المجموعة مع علامات تبويب معروفة
            tabStops.Clear();
            tabStops.Add(TextTabAlignmentType.Left, 50);
            tabStops.Add(TextTabAlignmentType.Center, 150);
            tabStops.Add(TextTabAlignmentType.Right, 250);

            try
            {
                // استخدم خاصية Item (المؤشر) لقراءة علامة تبويب محددة
                TextTabStop firstStop = tabStops[0]; // Item property (read‑only)
                Console.WriteLine($"First Tab Stop -> Position: {firstStop.TabPosition}, Alignment: {firstStop.TabAlignment}");

                // أظهر قراءة عنصر آخر
                TextTabStop secondStop = tabStops[1];
                Console.WriteLine($"Second Tab Stop -> Position: {secondStop.TabPosition}, Alignment: {secondStop.TabAlignment}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error accessing Item property: {ex.Message}");
            }

            // حفظ المصنف مع التغييرات
            workbook.Save("TextTabStopCollectionItemDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [TextTabStop](../../texttabstop/)
* class [TextTabStopCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


