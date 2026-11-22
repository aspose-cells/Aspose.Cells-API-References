---
title: "التعداد DynamicFilterType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.DynamicFilterType. نوع الفلتر الديناميكي"
type: docs
url: /ar/net/aspose.cells/dynamicfiltertype/
---
## DynamicFilterType enumeration

نوع الفلتر الديناميكي.

```csharp
public enum DynamicFilterType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| AboveAverage | `0` | يعرض القيم التي هي فوق المتوسط. |
| BelowAverage | `1` | يعرض القيم التي هي تحت المتوسط. |
| LastMonth | `2` | يعرض تواريخ الشهر الماضي. |
| LastQuarter | `3` | يعرض تواريخ الربع الأخير. |
| LastWeek | `4` | يعرض تواريخ الأسبوع الماضي. |
| LastYear | `5` | يعرض تواريخ السنة الماضية. |
| January | `6` | يعرض التواريخ التي تقع في يناير، بغض النظر عن السنة. |
| October | `7` | يعرض التواريخ التي تكون في أكتوبر، بغض النظر عن السنة. |
| November | `8` | يعرض التواريخ التي تكون في نوفمبر، بغض النظر عن السنة. |
| December | `9` | يعرض التواريخ التي تكون في ديسمبر، بغض النظر عن السنة. |
| February | `10` | يعرض التواريخ التي تكون في فبراير، بغض النظر عن السنة. |
| March | `11` | يعرض التواريخ التي تكون في مارس، بغض النظر عن السنة. |
| April | `12` | يعرض التواريخ التي تكون في أبريل، بغض النظر عن السنة. |
| May | `13` | يعرض التواريخ التي تكون في مايو، بغض النظر عن السنة. |
| June | `14` | يعرض التواريخ التي تكون في يونيو، بغض النظر عن السنة. |
| July | `15` | يعرض التواريخ التي تكون في يوليو، بغض النظر عن السنة. |
| August | `16` | يعرض التواريخ التي تكون في أغسطس، بغض النظر عن السنة. |
| September | `17` | يعرض التواريخ التي تكون في سبتمبر، بغض النظر عن السنة. |
| NextMonth | `18` | يعرض تواريخ الشهر القادم. |
| NextQuarter | `19` | يعرض تواريخ الربع القادم. |
| NextWeek | `20` | يعرض تواريخ الأسبوع القادم. |
| NextYear | `21` | يعرض تواريخ السنة القادمة. |
| None | `22` | لا شيء. |
| Quarter1 | `23` | يعرض التواريخ التي تكون في الربع الأول، بغض النظر عن السنة. |
| Quarter2 | `24` | يعرض التواريخ التي تكون في الربع الثاني، بغض النظر عن السنة. |
| Quarter3 | `25` | يعرض التواريخ التي تكون في الربع الثالث، بغض النظر عن السنة. |
| Quarter4 | `26` | يعرض التواريخ التي تكون في الربع الرابع، بغض النظر عن السنة. |
| ThisMonth | `27` | يعرض تواريخ هذا الشهر. |
| ThisQuarter | `28` | يعرض تواريخ هذا الربع. |
| ThisWeek | `29` | يعرض تواريخ هذا الأسبوع. |
| ThisYear | `30` | يعرض تواريخ هذه السنة. |
| Today | `31` | يعرض تواريخ اليوم. |
| Tomorrow | `32` | يعرض تواريخ الغد. |
| YearToDate | `33` | يعرض التواريخ بين بداية السنة واليوم، شاملًا. |
| Yesterday | `34` | يعرض تواريخ الأمس. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DynamicFilterTypeDemo
    {
        public static void DynamicFilterTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Date");
            worksheet.Cells["A2"].PutValue(new DateTime(2023, 1, 1));
            worksheet.Cells["A3"].PutValue(new DateTime(2023, 2, 1));
            worksheet.Cells["A4"].PutValue(new DateTime(2023, 3, 1));
            worksheet.Cells["A5"].PutValue(new DateTime(2023, 4, 1));
            worksheet.Cells["A6"].PutValue(new DateTime(2023, 5, 1));

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);
            worksheet.Cells["B6"].PutValue(50);

            // تطبيق الفلتر التلقائي على ورقة العمل
            worksheet.AutoFilter.SetRange(0, 0, 5);

            // تطبيق فلتر ديناميكي لعرض التواريخ في مارس فقط
            worksheet.AutoFilter.DynamicFilter(0, DynamicFilterType.March);

            // احفظ المصنف
            workbook.Save("DynamicFilterTypeExample.xlsx");
            workbook.Save("DynamicFilterTypeExample.pdf");

            // أخرج النتائج
            Console.WriteLine("Dynamic filter applied to show only dates in March.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


