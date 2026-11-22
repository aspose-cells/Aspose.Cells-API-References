---
title: "تعداد DisplayUnitType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.Charts.DisplayUnitType. يمثل نوع وحدة العرض لمحور المخططات"
type: docs
url: /ar/net/aspose.cells.charts/displayunittype/
---
## DisplayUnitType enumeration

يمثل نوع وحدة العرض لمحور المخطط.

```csharp
public enum DisplayUnitType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | وحدة العرض هي لا شيء. |
| Hundreds | `1` | يحدد أن القيم على المخطط يجب أن تُقسم على 100. |
| Thousands | `2` | يحدد أن القيم على المخطط يجب أن تُقسم على 1,000. |
| TenThousands | `3` | يحدد أن القيم على المخطط يجب أن تُقسم على 10,000. |
| HundredThousands | `4` | يحدد أن القيم على المخطط يجب أن تُقسم على 100,000. |
| Millions | `5` | يحدد أن القيم على المخطط يجب أن تُقسم على 1,000,000. |
| TenMillions | `6` | يحدد أن القيم على المخطط يجب أن تُقسم على 10,000,000. |
| HundredMillions | `7` | يحدد أن القيم على المخطط يجب أن تُقسم على 100,000,000. |
| Billions | `8` | يحدد أن القيم على المخطط يجب أن تُقسم على 1,000,000,000. |
| Trillions | `9` | يحدد أن القيم على المخطط يجب أن تُقسم على 1,000,000,000,000. |
| Percentage | `10` | القيم على المخطط يجب أن تُقسم على 0.01. |
| Cust | `11` | يحدد قيمة مخصصة لوحدة العرض. |
| Custom | `12` | يحدد قيمة مخصصة لوحدة العرض. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class DisplayUnitTypeDemo
    {
        public static void DisplayUnitTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إضافة ورقة عمل جديدة إلى المصنف
            int sheetIndex = workbook.Worksheets.Add();
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // إضافة بعض البيانات النموذجية إلى ورقة العمل
            worksheet.Cells["A1"].PutValue(500000);
            worksheet.Cells["A2"].PutValue(1000000);
            worksheet.Cells["A3"].PutValue(1500000);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(50);
            
            // إضافة مخطط إلى ورقة العمل
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // أضف NSeries (مصدر بيانات المخطط) إلى المخطط من الخلية \"A1\" إلى \"B3\"
            chart.NSeries.Add("A1:B3", true);
            
            // عيّن وحدة العرض لمحور القيم إلى الملايين
            chart.ValueAxis.DisplayUnit = DisplayUnitType.Millions;
            
            // اختياريًا، اعرض تسمية وحدة العرض
            chart.ValueAxis.IsDisplayUnitLabelShown = true;
            
            // احفظ المصنف
            workbook.Save("DisplayUnitTypeExample.xlsx");
            workbook.Save("DisplayUnitTypeExample.pdf");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


