---
title: "تعداد SparklinePresetStyleType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "عدد Aspose.Cells.Charts.SparklinePresetStyleType. يمثل أنواع الأنماط المسبقة للـ sparkline"
type: docs
url: /ar/net/aspose.cells.charts/sparklinepresetstyletype/
---
## SparklinePresetStyleType enumeration

يمثل أنواع الأنماط المسبقة للـ sparkline.

```csharp
public enum SparklinePresetStyleType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Style1 | `0` | النمط 1 |
| Style2 | `1` | النمط 2 |
| Style3 | `2` | النمط 3 |
| Style4 | `3` | النمط 4 |
| Style5 | `4` | النمط 5 |
| Style6 | `5` | النمط 6 |
| Style7 | `6` | النمط 7 |
| Style8 | `7` | النمط 8 |
| Style9 | `8` | النمط 9 |
| Style10 | `9` | النمط 10 |
| Style11 | `10` | النمط 11 |
| Style12 | `11` | النمط 12 |
| Style13 | `12` | النمط 13 |
| Style14 | `13` | النمط 14 |
| Style15 | `14` | النمط 15 |
| Style16 | `15` | النمط 16 |
| Style17 | `16` | النمط 17 |
| Style18 | `17` | النمط 18 |
| Style19 | `18` | النمط 19 |
| Style20 | `19` | النمط 20 |
| Style21 | `20` | النمط 21 |
| Style22 | `21` | النمط 22 |
| Style23 | `22` | النمط 23 |
| Style24 | `23` | النمط 24 |
| Style25 | `24` | النمط 25 |
| Style26 | `25` | النمط 26 |
| Style27 | `26` | النمط 27 |
| Style28 | `27` | النمط 28 |
| Style29 | `28` | النمط 29 |
| Style30 | `29` | النمط 30 |
| Style31 | `30` | النمط 31 |
| Style32 | `31` | النمط 32 |
| Style33 | `32` | النمط 33 |
| Style34 | `33` | النمط 34 |
| Style35 | `34` | النمط 35 |
| Style36 | `35` | النمط 36 |
| Custom | `36` | لا يوجد نمط مسبق. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklinePresetStyleTypeDemo
    {
        public static void SparklinePresetStyleTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة للمخططات الصغيرة
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(3);
            worksheet.Cells["D1"].PutValue(4);
            worksheet.Cells["E1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(5);
            worksheet.Cells["B2"].PutValue(4);
            worksheet.Cells["C2"].PutValue(3);
            worksheet.Cells["D2"].PutValue(2);
            worksheet.Cells["E2"].PutValue(1);

            // تحديد CellArea للمخططات الصغيرة
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 1;
            ca.StartColumn = 5;
            ca.EndColumn = 5;

            // إضافة المخططات الصغيرة إلى ورقة العمل
            int idx = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:E2", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[idx];
            group.Sparklines.Add("A1:E1", 0, 5);
            group.Sparklines.Add("A2:E2", 1, 5);

            // تعيين نوع النمط المسبق لمجموعة المخططات الصغيرة
            group.PresetStyle = SparklinePresetStyleType.Style5;

            // احفظ المصنف
            workbook.Save("SparklinePresetStyleTypeExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


