---
title: "FontSettingCollection.Replace"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة FontSettingCollection. استبدال النص"
type: docs
url: /ar/net/aspose.cells.drawing.texts/fontsettingcollection/replace/
---
## Replace(int, int, string) {#replace}

استبدل النص.

```csharp
public void Replace(int index, int count, string text)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| فهرس | Int32 | فهرس البداية. |
| عدد | Int32 | عدد الأحرف. |
| نص | String | النص. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class FontSettingCollectionMethodReplaceWithInt32Int32StringDemo
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
            fontSettingCollection.Text = "Original text to be modified";

            try
            {
                // استدعِ طريقة Replace لاستبدال 8 أحرف بدءًا من الفهرس 9 بالنص الجديد
                fontSettingCollection.Replace(9, 8, "replaced");

                // عرض النص المعدل
                Console.WriteLine("Text after replacement: " + fontSettingCollection.Text);

                // احفظ المصنف
                workbook.Save("FontSettingCollectionReplaceDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Replace method: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)

---

## Replace(string, string) {#replace_1}

استبدل النص.

```csharp
public void Replace(string oldValue, string newValue)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| oldValue | String | النص القديم. |
| newValue | String | النص الجديد. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class FontSettingCollectionMethodReplaceWithStringStringDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة شكل وتعيين النص
            Shape shape = worksheet.Shapes.AddTextBox(1, 0, 0, 100, 100, 100);
            shape.Text = "Sample text ３４ for replacement";
            
            // استبدال النص داخل الشكل
            shape.TextBody.Replace("３４", "ABC");
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FontSettingCollection](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


