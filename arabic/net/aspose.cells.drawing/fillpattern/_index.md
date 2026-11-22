---
title: "تعداد FillPattern"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Drawing.FillPattern. يحدد أنواع نمط تعبئة الشكل"
type: docs
url: /ar/net/aspose.cells.drawing/fillpattern/
---
## FillPattern enumeration

يسرد أنواع نمط تعبئة الشكل.

```csharp
public enum FillPattern
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | يمثل عدم وجود خلفية. |
| Solid | `1` | يمثل نمط صلب. |
| Gray5 | `2` | يمثل نمط رمادي 5٪. |
| Gray10 | `3` | يمثل نمط رمادي 10٪. |
| Gray20 | `4` | يمثل نمط رمادي 20٪. |
| Gray30 | `5` | يمثل نمط رمادي 30٪. |
| Gray40 | `6` | يمثل نمط رمادي 40٪. |
| Gray50 | `7` | يمثل نمط رمادي بنسبة 50٪. |
| Gray60 | `8` | يمثل نمط رمادي 60٪. |
| Gray70 | `9` | يمثل نمط رمادي 70٪. |
| Gray75 | `10` | يمثل نمط رمادي بنسبة 75٪. |
| Gray80 | `11` | يمثل نمط رمادي 80%. |
| Gray90 | `12` | يمثل نمط رمادي 90%. |
| Gray25 | `13` | يمثل نمط رمادي بنسبة 25٪. |
| LightDownwardDiagonal | `14` | يمثل نمط قطري مائل إلى الأسفل خفيف. |
| LightUpwardDiagonal | `15` | يمثل نمط قطري مائل إلى الأعلى خفيف. |
| DarkDownwardDiagonal | `16` | يمثل نمط قطري مائل إلى الأسفل غامق. |
| DarkUpwardDiagonal | `17` | يمثل نمط قطري مائل إلى الأعلى غامق. |
| WideDownwardDiagonal | `18` | يمثل نمط قطري مائل إلى الأسفل واسع. |
| WideUpwardDiagonal | `19` | يمثل نمط قطري مائل إلى الأعلى واسع. |
| LightVertical | `20` | يمثل نمط عمودي خفيف. |
| LightHorizontal | `21` | يمثل نمط أفقي خفيف. |
| NarrowVertical | `22` | يمثل نمط عمودي ضيق. |
| NarrowHorizontal | `23` | يمثل نمط أفقي ضيق. |
| DarkVertical | `24` | يمثل نمط عمودي غامق. |
| DarkHorizontal | `25` | يمثل نمط أفقي غامق. |
| DashedDownwardDiagonal | `26` | يمثل نمط قطري مائل إلى الأسفل متقطع. |
| DashedUpwardDiagonal | `27` | يمثل نمط قطري مائل إلى الأعلى متقطع. |
| DashedVertical | `28` | يمثل نمط عمودي متقطع. |
| DashedHorizontal | `29` | يمثل نمط أفقي متقطع. |
| SmallConfetti | `30` | يمثل نمط قنابل ورقية صغيرة. |
| LargeConfetti | `31` | يمثل نمط قنابل ورقية كبيرة. |
| ZigZag | `32` | يمثل نمط متعرج. |
| Wave | `33` | يمثل نمط موجي. |
| DiagonalBrick | `34` | يمثل نمط طوب قطري. |
| HorizontalBrick | `35` | يمثل نمط طوب أفقي. |
| Weave | `36` | يمثل نمط نسج. |
| Plaid | `37` | يمثل نمط مربعات. |
| Divot | `38` | يمثل نمط تجويف. |
| DottedGrid | `39` | يمثل نمط شبكة منقطة. |
| DottedDiamond | `40` | يمثل نمط ماسي منقّط. |
| Shingle | `41` | يمثل نمط ألواح. |
| Trellis | `42` | يمثل نمط شبيك. |
| Sphere | `43` | يمثل نمط كروي. |
| SmallGrid | `44` | يمثل نمط شبكة صغيرة. |
| LargeGrid | `45` | يمثل نمط شبكة كبيرة. |
| SmallCheckerBoard | `46` | يمثل نمط لوحة شطرنج صغيرة. |
| LargeCheckerBoard | `47` | يمثل نمط لوحة شطرنج كبيرة. |
| OutlinedDiamond | `48` | يمثل نمط ماسي محدد. |
| SolidDiamond | `49` | يمثل نمط ماسي صلب. |
| Unknown | `50` | يمثل نمط غير معروف. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassFillPatternDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // إضافة مخطط
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // تعيين نمط التعبئة للسلسلة الأولى
            Series series = chart.NSeries[0];
            series.Area.FillFormat.Pattern = FillPattern.Plaid;

            // احفظ المصنف
            workbook.Save("FillPatternDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


