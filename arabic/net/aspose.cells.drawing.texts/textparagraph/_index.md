---
title: "الفئة TextParagraph"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Drawing.Texts.TextParagraph class. تمثل إعداد الفقرة النصية"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textparagraph/
---
## TextParagraph class

يمثل إعداد فقرة النص.

```csharp
public class TextParagraph : FontSetting
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AlignmentType](../../aspose.cells.drawing.texts/textparagraph/alignmenttype/) { get; set; } | الحصول وتعيين نوع محاذاة النص الأفقية للفقرة. |
| [Bullet](../../aspose.cells.drawing.texts/textparagraph/bullet/) { get; } | الحصول على الرصاصة. |
| [Children](../../aspose.cells.drawing.texts/textparagraph/children/) { get; } | الحصول على جميع مقاطع النص في هذه الفقرة. إذا كانت هذه الفقرة فارغة، إرجاع الفقرة نفسها. |
| [DefaultTabSize](../../aspose.cells.drawing.texts/textparagraph/defaulttabsize/) { get; set; } | الحصول وتعيين الحجم الافتراضي لحرف الجدولة داخل هذه الفقرة. |
| [FirstLineIndent](../../aspose.cells.drawing.texts/textparagraph/firstlineindent/) { get; set; } | يحدد حجم المسافة البادئة التي سيتم تطبيقها على السطر الأول من النص في الفقرة. |
| [Font](../../aspose.cells/fontsetting/font/) { get; } | يعيد الخط لهذا الكائن. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [FontAlignType](../../aspose.cells.drawing.texts/textparagraph/fontaligntype/) { get; set; } | يحدد موضع الكلمات الفعلية عموديًا على سطر النص. يتعامل هذا مع وضعية الأحرف عموديًا بالنسبة للخط الأساسي. |
| [IsEastAsianLineBreak](../../aspose.cells.drawing.texts/textparagraph/iseastasianlinebreak/) { get; set; } | يحدد ما إذا كان يمكن كسر كلمة شرق آسيوية إلى نصفين وتغليفها إلى السطر التالي دون إضافة شرطة. |
| [IsHangingPunctuation](../../aspose.cells.drawing.texts/textparagraph/ishangingpunctuation/) { get; set; } | يحدد ما إذا كان يجب وضع علامات الترقيم بقوة على سطر النص أو وضعها على سطر نص مختلف. |
| [IsLatinLineBreak](../../aspose.cells.drawing.texts/textparagraph/islatinlinebreak/) { get; set; } | يحدد ما إذا كان يمكن كسر كلمة لاتينية إلى نصفين وتغليفها إلى السطر التالي دون إضافة شرطة. |
| [LeftMargin](../../aspose.cells.drawing.texts/textparagraph/leftmargin/) { get; set; } | يحدد الهامش الأيسر للفقرة. |
| [Length](../../aspose.cells/fontsetting/length/) { get; } | يحصل على طول الأحرف. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [LineSpace](../../aspose.cells.drawing.texts/textparagraph/linespace/) { get; set; } | الحصول وتعيين مقدار المسافة البيضاء العمودية التي سيتم استخدامها داخل الفقرة. |
| [LineSpaceSizeType](../../aspose.cells.drawing.texts/textparagraph/linespacesizetype/) { get; set; } | الحصول وتعيين مقدار المسافة البيضاء العمودية التي سيتم استخدامها داخل الفقرة. |
| [RightMargin](../../aspose.cells.drawing.texts/textparagraph/rightmargin/) { get; set; } | يحدد الهامش الأيمن للفقرة. |
| [SpaceAfter](../../aspose.cells.drawing.texts/textparagraph/spaceafter/) { get; set; } | يحصل على ويضبط مقدار المسافة الرأسية الفارغة التي ستكون موجودة بعد الفقرة. |
| [SpaceAfterSizeType](../../aspose.cells.drawing.texts/textparagraph/spaceaftersizetype/) { get; set; } | يحصل على ويضبط مقدار المسافة الرأسية الفارغة التي ستكون موجودة بعد الفقرة. |
| [SpaceBefore](../../aspose.cells.drawing.texts/textparagraph/spacebefore/) { get; set; } | يحصل على ويضبط مقدار المسافة الرأسية الفارغة التي ستكون موجودة قبل الفقرة. |
| [SpaceBeforeSizeType](../../aspose.cells.drawing.texts/textparagraph/spacebeforesizetype/) { get; set; } | يحصل على ويضبط مقدار المسافة الرأسية الفارغة التي ستكون موجودة قبل الفقرة. |
| [StartIndex](../../aspose.cells/fontsetting/startindex/) { get; } | يحصل على الفهرس الابتدائي للأحرف. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| [Stops](../../aspose.cells.drawing.texts/textparagraph/stops/) { get; } | يحصل على قائمة نقاط التبويب. |
| [TextOptions](../../aspose.cells/fontsetting/textoptions/) { get; } | يعيد خيارات النص. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |
| override [Type](../../aspose.cells.drawing.texts/textparagraph/type/) { get; } | يحصل على نوع عقدة النص. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [SetWordArtStyle](../../aspose.cells/fontsetting/setwordartstyle/)(PresetWordArtStyle) | تعيين نمط WordArt المسبق. (موروث من [`FontSetting`](../../aspose.cells/fontsetting/).) |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class TextsClassTextParagraphDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة مربع نص إلى ورقة العمل
            int textBoxIndex = sheet.TextBoxes.Add(10, 10, 200, 100);
            Aspose.Cells.Drawing.TextBox textBox = sheet.TextBoxes[textBoxIndex];
            
            // تعيين محتوى النص مع فقرات متعددة
            textBox.Text = "First paragraph\nSecond paragraph\nThird paragraph";

            // الوصول إلى فقرات النص وتعديلها
            foreach (TextParagraph paragraph in textBox.TextBody.TextParagraphs)
            {
                // تعيين خصائص الفقرة
                paragraph.LineSpaceSizeType = LineSpaceSizeType.Points;
                paragraph.LineSpace = 20;
                paragraph.AlignmentType = TextAlignmentType.Center;
            }

            // احفظ المصنف
            workbook.Save("TextParagraphDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [FontSetting](../../aspose.cells/fontsetting/)
* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


