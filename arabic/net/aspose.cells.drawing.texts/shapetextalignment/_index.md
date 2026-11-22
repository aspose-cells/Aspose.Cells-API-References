---
title: "الفئة ShapeTextAlignment"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Drawing.Texts.ShapeTextAlignment. تمثّل إعداد محاذاة نص الأشكال"
type: docs
url: /ar/net/aspose.cells.drawing.texts/shapetextalignment/
---
## ShapeTextAlignment class

يمثل إعداد محاذاة نص الشكل؛

```csharp
public class ShapeTextAlignment
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [AutoSize](../../aspose.cells.drawing.texts/shapetextalignment/autosize/) { get; set; } | يشير إلى ما إذا كان حجم الشكل يتم ضبطه تلقائيًا وفقًا لمحتواه. |
| [BottomMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/bottommarginpt/) { get; set; } | يعيد الهامش السفلي بوحدة النقاط |
| [IsAutoMargin](../../aspose.cells.drawing.texts/shapetextalignment/isautomargin/) { get; set; } | يشير إلى ما إذا كان هامش إطار النص تلقائيًا. |
| [IsLockedText](../../aspose.cells.drawing.texts/shapetextalignment/islockedtext/) { get; set; } | يشير إلى ما إذا كان الشكل مقفلًا عندما تكون ورقة العمل محمية. |
| [IsTextWrapped](../../aspose.cells.drawing.texts/shapetextalignment/istextwrapped/) { get; set; } | يحصل على أو يضبط نوع التفاف النص للشكل الذي يحتوي على نص. |
| [LeftMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/leftmarginpt/) { get; set; } | يعيد الهامش الأيسر بوحدة النقاط |
| [NumberOfColumns](../../aspose.cells.drawing.texts/shapetextalignment/numberofcolumns/) { get; set; } | يحصل على ويضبط عدد أعمدة النص في المستطيل المحيط. |
| [RightMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/rightmarginpt/) { get; set; } | يعيد الهامش الأيمن بوحدة النقاط |
| [RotateTextWithShape](../../aspose.cells.drawing.texts/shapetextalignment/rotatetextwithshape/) { get; set; } | يشير إلى ما إذا كان يتم تدوير النص مع الشكل. |
| [RotationAngle](../../aspose.cells.drawing.texts/shapetextalignment/rotationangle/) { get; set; } | يحصل على ويضبط دوران الشكل. |
| [TextHorizontalOverflow](../../aspose.cells.drawing.texts/shapetextalignment/texthorizontaloverflow/) { get; set; } | يحصل على ويضبط نوع تجاوز النص الأفقي لمربع النص. |
| [TextShapeType](../../aspose.cells.drawing.texts/shapetextalignment/textshapetype/) { get; set; } | يحصل على ويضبط نوع تحويل النص. |
| [TextVerticalOverflow](../../aspose.cells.drawing.texts/shapetextalignment/textverticaloverflow/) { get; set; } | يحصل على ويضبط نوع تجاوز النص العمودي لمربع النص. |
| [TextVerticalType](../../aspose.cells.drawing.texts/shapetextalignment/textverticaltype/) { get; set; } | يحصل على ويضبط اتجاه النص. |
| [TopMarginPt](../../aspose.cells.drawing.texts/shapetextalignment/topmarginpt/) { get; set; } | يعيد الهامش العلوي بوحدة النقاط |

## الطرق

| الاسم | الوصف |
| --- | --- |
| override [Equals](../../aspose.cells.drawing.texts/shapetextalignment/equals/)(object) | يحدد ما إذا كانت هذه المثيلة لها نفس القيمة مثل كائن `ShapeTextAlignment` المحدد الآخر. |
| override [GetHashCode](../../aspose.cells.drawing.texts/shapetextalignment/gethashcode/)() |  |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class ShapeTextAlignmentDemo
    {
        public static void ShapeTextAlignmentExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);

            // الوصول إلى كائن ShapeTextAlignment
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // ضبط الخصائص
            shapeTextAlignment.IsTextWrapped = true;
            shapeTextAlignment.RotateTextWithShape = true;
            shapeTextAlignment.TextVerticalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.TextHorizontalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.RotationAngle = 90;
            shapeTextAlignment.TextVerticalType = TextVerticalType.Horizontal;
            shapeTextAlignment.IsLockedText = false;
            shapeTextAlignment.AutoSize = false;
            shapeTextAlignment.TextShapeType = AutoShapeType.TextBox;
            shapeTextAlignment.TopMarginPt = 2.0d;
            shapeTextAlignment.BottomMarginPt = 2.0d;
            shapeTextAlignment.LeftMarginPt = 2.0d;
            shapeTextAlignment.RightMarginPt = 2.0d;
            shapeTextAlignment.IsAutoMargin = true;
            shapeTextAlignment.NumberOfColumns = 1;

            // حفظ المصنف
            workbook.Save("ShapeTextAlignmentExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


