---
title: "التعداد TextNodeType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.Texts.TextNodeType. يمثل نوع العقدة"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textnodetype/
---
## TextNodeType enumeration

يمثل نوع العقدة.

```csharp
public enum TextNodeType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| TextRun | `0` | يمثل عقدة النص. |
| TextParagraph | `1` | يمثل فقرة النص. |
| Equation | `2` | يمثل نص المعادلة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextsClassTextNodeTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء صندوق نص والحصول على فقرات النص الخاصة به
            int textboxIndex = worksheet.TextBoxes.Add(10, 10, 200, 100);
            Aspose.Cells.Drawing.TextBox textbox = worksheet.TextBoxes[textboxIndex];
            textbox.TextBody.AppendText("Sample text with ");
            textbox.TextBody.AppendText("different node types");
            
            // عرض استخدام TextNodeType
            foreach (TextParagraph paragraph in textbox.TextBody.TextParagraphs)
            {
                foreach (FontSetting portion in paragraph.Children)
                {
                    // احصل على جزء النص باستخدام StartIndex و Length
                    string portionText = textbox.Text.Substring(portion.StartIndex, portion.Length);
                    Console.WriteLine("Text: " + portionText);
                    Console.WriteLine("Node Type: " + portion.Type.ToString());
                    
                    // مثال على فحص نوع العقدة
                    if (portion.Type == TextNodeType.TextRun)
                    {
                        portion.Font.Color = System.Drawing.Color.Red;
                    }
                    else if (portion.Type == TextNodeType.Equation)
                    {
                        portion.Font.Color = System.Drawing.Color.Blue;
                    }
                }
            }

            // حفظ النتيجة
            workbook.Save("TextNodeTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


