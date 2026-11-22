---
title: "الفئة TextParagraphCollection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.Texts.TextParagraphCollection. تمثل جميع فقرات النص"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textparagraphcollection/
---
## TextParagraphCollection class

يمثل جميع فقرات النص.

```csharp
public class TextParagraphCollection : IEnumerable
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Count](../../aspose.cells.drawing.texts/textparagraphcollection/count/) { get; } | يحصل على عدد فقرات النص. |
| [Item](../../aspose.cells.drawing.texts/textparagraphcollection/item/) { get; } | يحصل على كائن [`TextParagraph`](../textparagraph/) في الفهرس المحدد. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [GetEnumerator](../../aspose.cells.drawing.texts/textparagraphcollection/getenumerator/)() | يسترجع عداد الفقرات. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassTextParagraphCollectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // أضف مربع نص إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddTextBox(0, 0, 0, 0, 400, 400);
            
            // عيّن نصًا متعدد الأسطر
            shape.Text = "First paragraph\nSecond paragraph";
            
            // احصل على مجموعة الفقرات
            TextParagraphCollection paragraphs = shape.TextBody.TextParagraphs;
            
            // الوصول إلى الفقرة الثانية وتعديلها
            TextParagraph secondParagraph = paragraphs[1];
            secondParagraph.LineSpaceSizeType = LineSpaceSizeType.Points;
            secondParagraph.LineSpace = 20;
            secondParagraph.SpaceAfter = 30;
            secondParagraph.SpaceBefore = 40;
            
            // احفظ المصنف
            workbook.Save("TextParagraphCollectionDemo.xlsx");
            
            Console.WriteLine("Text paragraph formatting saved successfully.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


