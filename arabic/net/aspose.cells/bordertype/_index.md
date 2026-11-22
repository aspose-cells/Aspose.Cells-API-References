---
title: "تعداد BorderType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.BorderType. يعدد أنواع خطوط الحدود والخطوط القطرية"
type: docs
url: /ar/net/aspose.cells/bordertype/
---
## BorderType enumeration

يسرد أنواع خطوط الحدود والخطوط القطرية.

```csharp
[Flags]
public enum BorderType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| LeftBorder | `1` | يمثل خط الحد الأيسر. |
| RightBorder | `2` | يمثل وجود خط الحد الأيمن. |
| TopBorder | `4` | يمثل خط الحد العلوي. |
| BottomBorder | `8` | يمثل خط الحد السفلي. |
| DiagonalDown | `10` | يمثل الخط القطري من الأعلى الأيسر إلى الأسفل الأيمن. |
| DiagonalUp | `20` | يمثل الخط القطري من الأسفل الأيسر إلى الأعلى الأيمن. |
| Vertical | `40` | فقط للأنماط الديناميكية، مثل التنسيق الشرطي، وجداول المحور. |
| Horizontal | `80` | فقط للأنماط الديناميكية، مثل التنسيق الشرطي، وجداول المحور. |
| SideBorders | `F` | يشير إلى حدود الأربعة الجوانب: LeftBorder، RightBorder، TopBorder و BottomBorder. |
| Diagonal | `30` | تركيبة خاصة من حدود متعددة لراحة المستخدم لبعض واجهات برمجة التطبيقات. يشير إلى الحدود القطرية DiagonalUp و DiagonalDown. |
| DynamicStyleBorders | `C0` | يشير إلى العمودي والأفقي للأنماط الديناميكية. |
| None | `0` | لم يتم تحديد أي حد. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BorderTypeDemo
    {
        public static void BorderTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            // إنشاء نطاق من الخلايا
            var range = worksheet.Cells.CreateRange("A1:D4");

            // إنشاء كائن نمط
            Style style = workbook.CreateStyle();
            // تعيين الحدود للنطاق
            style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Black);
            style.SetBorder(BorderType.DiagonalDown, CellBorderType.Thin, Color.Red);
            style.SetBorder(BorderType.DiagonalUp, CellBorderType.Thin, Color.Blue);

            // تطبيق النمط على النطاق
            StyleFlag flag = new StyleFlag { Borders = true };
            range.ApplyStyle(style, flag);

            // احفظ المصنف
            workbook.Save("BorderTypeExample.xlsx");
            workbook.Save("BorderTypeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


