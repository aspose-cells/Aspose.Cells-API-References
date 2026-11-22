---
title: "تعداد TextVerticalType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.Drawing.Texts.TextVerticalType. يمثل نوع اتجاه النص"
type: docs
url: /ar/net/aspose.cells.drawing.texts/textverticaltype/
---
## TextVerticalType enumeration

يمثل نوع توجيه النص.

```csharp
public enum TextVerticalType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Vertical | `0` | عرض عمودي للشرق الآسيوي. |
| Horizontal | `1` | نص أفقي. |
| VerticalLeftToRight | `2` | يُعرض عموديًا ويتدفق النص من الأعلى إلى الأسفل ثم من اليسار إلى اليمين |
| Vertical90 | `3` | كل سطر يدور 90 درجة مع اتجاه عقارب الساعة |
| Vertical270 | `4` | كل سطر يدور 270 درجة مع اتجاه عقارب الساعة |
| Stacked | `5` | يحدد ما إذا كان كل النص عموديًا |
| StackedRightToLeft | `6` | يحدد أن WordArt العمودي يجب أن يُعرض من اليمين إلى اليسار بدلاً من اليسار إلى اليمين. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class TextVerticalTypeDemo
    {
        public static void TextVerticalTypeExample()
        {
            // إنشاء كائن Workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة شكل مستطيل إلى ورقة العمل
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);

            // الوصول إلى إعدادات محاذاة النص للشكل
            ShapeTextAlignment shapeTextAlignment = shape.TextBody.TextAlignment;

            // تعيين نوع النص العمودي إلى أفقي
            shapeTextAlignment.TextVerticalType = TextVerticalType.Horizontal;

            // تعيين خصائص أخرى للعرض
            shapeTextAlignment.IsTextWrapped = true;
            shapeTextAlignment.RotateTextWithShape = true;
            shapeTextAlignment.TextVerticalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.TextHorizontalOverflow = TextOverflowType.Clip;
            shapeTextAlignment.RotationAngle = 90;
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
            workbook.Save("TextVerticalTypeExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing.Texts](../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../)


