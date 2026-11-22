---
title: "تعداد BackgroundType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.BackgroundType. يعدد أنواع أنماط خلفية الخلية."
type: docs
url: /ar/net/aspose.cells/backgroundtype/
---
## BackgroundType enumeration

يسرد أنواع نمط خلفية الخلية.

```csharp
public enum BackgroundType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| DiagonalCrosshatch | `9` | يمثل نمط الترصيع المائل. |
| DiagonalStripe | `8` | يمثل نمط الشريط المائل. |
| Gray6 | `18` | يمثل نمط رمادي بنسبة 6.25٪. |
| Gray12 | `17` | يمثل نمط رمادي بنسبة 12.5٪. |
| Gray25 | `4` | يمثل نمط رمادي بنسبة 25٪. |
| Gray50 | `2` | يمثل نمط رمادي بنسبة 50٪. |
| Gray75 | `3` | يمثل نمط رمادي بنسبة 75٪. |
| HorizontalStripe | `5` | يمثل نمط الشريط الأفقي. |
| None | `0` | يمثل عدم وجود خلفية. |
| ReverseDiagonalStripe | `7` | يمثل نمط الشريط المائل العكسي. |
| Solid | `1` | يمثل نمط صلب. |
| ThickDiagonalCrosshatch | `10` | يمثل نمط الترصيع المائل السميك. |
| ThinDiagonalCrosshatch | `16` | يمثل نمط الترصيع المائل الرقيق. |
| ThinDiagonalStripe | `14` | يمثل نمط الشريط المائل الرقيق. |
| ThinHorizontalCrosshatch | `15` | يمثل نمط الترصيع الأفقي الرقيق. |
| ThinHorizontalStripe | `11` | يمثل نمط الشريط الأفقي الرقيق. |
| ThinReverseDiagonalStripe | `13` | يمثل نمط الشريط المائل العكسي الرقيق. |
| ThinVerticalStripe | `12` | يمثل نمط شريط عمودي رفيع. |
| VerticalStripe | `6` | يمثل نمط شريط عمودي. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class BackgroundTypeDemo
    {
        public static void BackgroundTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى في المصنف
            Worksheet worksheet = workbook.Worksheets[0];
            
            // الوصول إلى خلية من ورقة العمل
            Cell cell = worksheet.Cells["A1"];
            
            // تعيين قيمة الخلية
            cell.PutValue("Hello, Aspose!");

            // إنشاء كائن نمط
            Style style = cell.GetStyle();
            
            // تعيين نوع نمط الخلفية
            style.Pattern = BackgroundType.DiagonalStripe;
            
            // تعيين لون المقدمة
            style.ForegroundColor = Color.Red;
            
            // تعيين لون الخلفية
            style.BackgroundColor = Color.Green;
            
            // تطبيق النمط على الخلية
            cell.SetStyle(style);
            
            // احفظ المصنف
            workbook.Save("BackgroundTypeExample.xlsx");
            workbook.Save("BackgroundTypeExample.pdf");



        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


