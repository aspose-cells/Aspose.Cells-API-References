---
title: "تعداد DataBarBorderType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.DataBarBorderType تعداد. يحدد نوع حد شريط البيانات"
type: docs
url: /ar/net/aspose.cells/databarbordertype/
---
## DataBarBorderType enumeration

يحدد نوع حدود شريط البيانات.

```csharp
public enum DataBarBorderType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | شريط البيانات لا يحتوي على حد. |
| Solid | `1` | شريط البيانات يحتوي على حد صلب. |

### أمثلة

```csharp
using Aspose.Cells;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarBorderTypeDemo
    {
        public static void DataBarBorderTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // إضافة تنسيق شرطي إلى ورقة العمل
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[index];

            // تحديد نطاق خلايا للتنسيق الشرطي
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 3,
                StartColumn = 0,
                EndColumn = 0
            };
            fcc.AddArea(ca);

            // إضافة قاعدة تنسيق شرطي لشريط البيانات
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];

            // الوصول إلى كائن DataBar
            DataBar dataBar = fc.DataBar;

            // تعيين لون شريط البيانات
            dataBar.Color = Color.Blue;

            // تعيين الحد الأدنى والحد الأقصى لطول شريط البيانات
            dataBar.MinLength = 10;
            dataBar.MaxLength = 90;

            // تعيين نوع حد شريط البيانات
            dataBar.BarBorder.Type = DataBarBorderType.Solid;

            // تعيين لون حد شريط البيانات
            dataBar.BarBorder.Color = Color.Red;

            // احفظ المصنف
            workbook.Save("DataBarBorderTypeExample.xlsx");
            workbook.Save("DataBarBorderTypeExample.pdf");

            Console.WriteLine("DataBarBorderTypeExample executed successfully.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


