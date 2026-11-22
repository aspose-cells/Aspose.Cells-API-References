---
title: "FontSettingCollection.AppendText"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FontSettingCollection. تُضيف النص"
type: docs
url: /ar/net/aspose.cells.drawing.texts/fontsettingcollection/appendtext/
---
## FontSettingCollection.AppendText method

يضيف النص.

```csharp
public void AppendText(string text)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | String | النص. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodAppendTextWithStringDemo
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
            fontSettingCollection.Text = "Hello, ";

            try
            {
                // استدعاء طريقة AppendText لإضافة نص إضافي
                fontSettingCollection.AppendText("World!");

                // عرض النص المعدل
                Console.WriteLine("Text after append: " + fontSettingCollection.Text);

                // احفظ المصنف
                workbook.Save("FontSettingCollectionAppendTextDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing AppendText method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


