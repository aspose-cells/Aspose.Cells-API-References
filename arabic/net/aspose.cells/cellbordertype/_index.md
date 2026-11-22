---
title: "Enum CellBorderType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.CellBorderType enum. يعدد نوع حدود الخلايا"
type: docs
url: /ar/net/aspose.cells/cellbordertype/
---
## CellBorderType enumeration

يسرد نوع حدود الخلية.

```csharp
public enum CellBorderType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| DashDot | `9` | يمثل خطًا رفيعًا منقّطًا ومتقطعًا |
| DashDotDot | `11` | يمثل خطًا رفيعًا منقّطًا-متقطعًا |
| Dashed | `3` | يمثل خطًا متقطعًا |
| Dotted | `4` | يمثل خطًا منقطًا. |
| Double | `6` | يمثل خطًا مزدوجًا |
| Hair | `7` | يمثل خطًا رفيعًا. |
| MediumDashDot | `10` | يمثل خطًا متوسطًا منقّطًا ومتقطعًا |
| MediumDashDotDot | `12` | يمثل خطًا متوسطًا منقّطًا-متقطعًا |
| MediumDashed | `8` | يمثل خطًا متوسطًا متقطعًا |
| None | `0` | يمثل عدم وجود خط |
| Medium | `2` | يمثل خطًا متوسطًا |
| SlantedDashDot | `13` | يمثل خطًا مائلًا متوسطًا منقّطًا ومتقطعًا |
| Thick | `5` | يمثل خطًا سميكًا |
| Thin | `1` | يمثل خطًا رفيعًا |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class CellBorderTypeDemo
    {
        public static void CellBorderTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نطاق (A1:D4)
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1", "D4");

            // احصل على نمط النطاق
            Style style = workbook.CreateStyle();

            // تعيين أنماط حدود مختلفة للنطاق
            style.Borders[BorderType.TopBorder].LineStyle = CellBorderType.Thick;
            style.Borders[BorderType.TopBorder].Color = Color.Black;

            style.Borders[BorderType.BottomBorder].LineStyle = CellBorderType.Dashed;
            style.Borders[BorderType.BottomBorder].Color = Color.Blue;

            style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Dotted;
            style.Borders[BorderType.LeftBorder].Color = Color.Green;

            style.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Double;
            style.Borders[BorderType.RightBorder].Color = Color.Red;

            // تطبيق النمط على النطاق
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.Borders = true;
            range.ApplyStyle(style, styleFlag);

            // احفظ المصنف
            workbook.Save("CellBorderTypeExample.xlsx");
            workbook.Save("CellBorderTypeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


