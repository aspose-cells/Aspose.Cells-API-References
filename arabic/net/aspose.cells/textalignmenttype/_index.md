---
title: "تعداد TextAlignmentType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.TextAlignmentType. يُعدد أنواع محاذاة النص"
type: docs
url: /ar/net/aspose.cells/textalignmenttype/
---
## TextAlignmentType enumeration

يسرد أنواع محاذاة النص.

```csharp
public enum TextAlignmentType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| General | `1792` | يمثل محاذاة النص العامة. |
| Bottom | `528` | يمثل محاذاة النص السفلية. |
| Center | `1802` | يمثل محاذاة النص الوسطية. |
| CenterAcross | `1286` | يمثل محاذاة النص عبر الوسط. |
| Distributed | `807` | يمثل محاذاة النص الموزعة. |
| Fill | `1284` | يمثل محاذاة النص التعبئة. |
| Justify | `1821` | يمثل محاذاة النص المبررة. |
| Left | `257` | يمثل محاذاة النص اليسارية. |
| Right | `259` | يمثل محاذاة النص إلى اليمين. |
| Top | `512` | يمثل محاذاة النص إلى الأعلى. |
| JustifiedLow | `832` | يضبط النص بطول كاشدة معدل للنص العربي. |
| ThaiDistributed | `896` | يوزع النص التايلاندي بشكل خاص، لأن كل حرف يُعامل ككلمة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class TextAlignmentTypeDemo
    {
        public static void TextAlignmentTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(78);

            // إضافة تعليق إلى خلية
            Comment comment = worksheet.Comments[worksheet.Comments.Add("A1")];
            comment.Note = "This is a comment.";
            comment.TextHorizontalAlignment = TextAlignmentType.Center;
            comment.TextVerticalAlignment = TextAlignmentType.Top;

            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // تعيين نطاق بيانات المخطط
            chart.SetChartDataRange("A1:B4", true);

            // تخصيص عنوان المخطط
            chart.Title.Text = "Scores Chart";
            chart.Title.TextHorizontalAlignment = TextAlignmentType.Center;
            chart.Title.TextVerticalAlignment = TextAlignmentType.Top;

            // احفظ المصنف
            workbook.Save("TextAlignmentTypeExample.xlsx");

            // أخرج النتائج
            Console.WriteLine("Workbook saved successfully with text alignment settings.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


