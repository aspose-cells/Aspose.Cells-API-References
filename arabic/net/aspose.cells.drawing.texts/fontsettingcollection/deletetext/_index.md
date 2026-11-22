---
title: "FontSettingCollection.DeleteText"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FontSettingCollection. حذف بعض الأحرف"
type: docs
url: /ar/net/aspose.cells.drawing.texts/fontsettingcollection/deletetext/
---
## FontSettingCollection.DeleteText method

احذف بعض الأحرف.

```csharp
public void DeleteText(int index, int count)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | فهرس البداية. |
| عدد | Int32 | عدد الأحرف. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodDeleteTextWithInt32Int32Demo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة مربع نص إلى ورقة العمل
            var textBox = worksheet.Shapes.AddTextBox(0, 0, 100, 100, 200, 200);
            var fontSettingCollection = textBox.TextBody;

            // حدد النص الأولي
            fontSettingCollection.Text = "This is sample text to demonstrate DeleteText method";

            try
            {
                // عرض النص الأصلي
                Console.WriteLine("Original text: " + fontSettingCollection.Text);

                // استدعِ طريقة DeleteText لإزالة 7 أحرف بدءًا من الفهرس 5
                fontSettingCollection.DeleteText(5, 7);

                // عرض النص المعدل
                Console.WriteLine("Text after deletion: " + fontSettingCollection.Text);

                // احفظ المصنف
                workbook.Save("FontSettingCollectionDeleteTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing DeleteText method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


