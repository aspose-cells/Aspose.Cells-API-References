---
title: "تعداد TextureType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Drawing.TextureType. يمثل نوع النسيج المحدد مسبقًا"
type: docs
url: /ar/net/aspose.cells.drawing/texturetype/
---
## TextureType enumeration

يمثل نوع النسيج المحدد مسبقاً.

```csharp
public enum TextureType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| BlueTissuePaper | `0` | يمثل نوع نسيج الورق النسيجي الأزرق. |
| Bouquet | `1` | يمثل نوع نسيج الباقة. |
| BrownMarble | `2` | يمثل نوع نسيج الرخام البني. |
| Canvas | `3` | يمثل نوع نسيج القماش. |
| Cork | `4` | يمثل نوع نسيج الفلين. |
| Denim | `5` | يمثل نوع نسيج الدنيم. |
| FishFossil | `6` | يمثل نوع نسيج أحفاة السمك. |
| Granite | `7` | يمثل نوع نسيج الغرانيت. |
| GreenMarble | `8` | يمثل نوع نسيج الرخام الأخضر. |
| MediumWood | `9` | يمثل نوع نسيج الخشب المتوسط. |
| Newsprint | `10` | يمثل نوع نسيج ورق الصحف. |
| Oak | `11` | يمثل نوع نسيج البلوط. |
| PaperBag | `12` | يمثل نوع نسيج حقيبة الورق. |
| Papyrus | `13` | يمثل نوع نسيج البردي. |
| Parchment | `14` | يمثل نوع نسيج الرق. |
| PinkTissuePaper | `15` | يمثل نوع نسيج الورق النسيجي الوردي. |
| PurpleMesh | `16` | يمثل نوع نسيج الشبكة الأرجوانية. |
| RecycledPaper | `17` | يمثل نوع نسيج الورق المعاد تدويره. |
| Sand | `18` | يمثل نوع نسيج الرمل. |
| Stationery | `19` | يمثل نوع نسيج القرطاسية. |
| Walnut | `20` | يمثل نوع نسيج قطرات الجوز. |
| WaterDroplets | `21` | يمثل نوع نسيج قطرات الماء. |
| WhiteMarble | `22` | يمثل نوع نسيج الرخام الأبيض. |
| WovenMat | `23` | يمثل نوع نسيج الحصيرة المنسوجة. |
| Unknown | `24` | يمثل نوع نسيج غير معروف. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassTextureTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // إضافة بيانات نموذجية للمخطط
            sheet.Cells["A1"].PutValue("Item");
            sheet.Cells["A2"].PutValue("Product A");
            sheet.Cells["A3"].PutValue("Product B");
            sheet.Cells["A4"].PutValue("Product C");
            sheet.Cells["B1"].PutValue("Sales");
            sheet.Cells["B2"].PutValue(1000);
            sheet.Cells["B3"].PutValue(2000);
            sheet.Cells["B4"].PutValue(3000);

            // إضافة مخطط
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // تعيين نطاق بيانات المخطط
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // الوصول إلى السلسلة الأولى وتعيين النسيج لنقطة
            ChartPoint point = chart.NSeries[0].Points[2];
            point.Area.FillFormat.Texture = TextureType.Stationery;

            // احفظ المصنف
            workbook.Save("TextureTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


