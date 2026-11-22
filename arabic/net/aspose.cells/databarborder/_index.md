---
title: "الفئة DataBarBorder"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.DataBarBorder. تمثل حد أشرطة البيانات المحددة بواسطة قاعدة تنسيق شرطي"
type: docs
url: /ar/net/aspose.cells/databarborder/
---
## DataBarBorder class

يمثل حد شريط البيانات المحدد بواسطة قاعدة تنسيق الخلايا الشرطي.

```csharp
public class DataBarBorder
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Color](../../aspose.cells/databarborder/color/) { get; set; } | يحصل أو يعيّن لون حد أشرطة البيانات المحددة بواسطة قاعدة تنسيق شرطي. |
| [Type](../../aspose.cells/databarborder/type/) { get; set; } | يحصل أو يعيّن نوع حد أشرطة البيانات المحددة بواسطة قاعدة تنسيق شرطي. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Drawing;

    public class DataBarBorderDemo
    {
        public static void DataBarBorderExample()
        {
            // إنشاء مصنف جديد
            Workbook workbook = new Workbook();
            // الوصول إلى ورقة العمل الأولى في المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بعض البيانات النموذجية إلى ورقة العمل
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(50);
            worksheet.Cells["A3"].PutValue(80);
            worksheet.Cells["A4"].PutValue(60);
            worksheet.Cells["A5"].PutValue(30);

            // إضافة تنسيق شرطي فارغ
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // تحديد نطاق خلايا للتنسيق الشرطي
            CellArea ca = new CellArea { StartRow = 0, EndRow = 4, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(ca);

            // إضافة شرط من نوع DataBar
            int conditionIndex = fcs.AddCondition(FormatConditionType.DataBar);
            FormatCondition formatCondition = fcs[conditionIndex];

            // الوصول إلى DataBar
            DataBar dataBar = formatCondition.DataBar;

            // تعيين خصائص DataBar
            dataBar.Color = Color.Orange;
            dataBar.MinCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MinCfvo.Value = 0;
            dataBar.MaxCfvo.Type = FormatConditionValueType.Percentile;
            dataBar.MaxCfvo.Value = 100;
            dataBar.ShowValue = true;

            // الوصول إلى خصائص DataBarBorder وتعيينها
            DataBarBorder dataBarBorder = dataBar.BarBorder;
            dataBarBorder.Type = DataBarBorderType.Solid;
            dataBarBorder.Color = Color.Black;

            // حفظ ملف Excel
            workbook.Save("DataBarBorderExample.xlsx");
            workbook.Save("DataBarBorderExample.pdf");

            Console.WriteLine("DataBar border example created successfully.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


