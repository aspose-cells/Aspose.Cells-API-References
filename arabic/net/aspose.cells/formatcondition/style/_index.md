---
title: "FormatCondition.Style"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية FormatCondition. يحصل أو يضبط نمط نطاقات الخلايا المشروطة"
type: docs
url: /ar/net/aspose.cells/formatcondition/style/
---
## FormatCondition.Style property

يحصل أو يضبط نمط نطاقات الخلايا المُنسقة شرطياً

```csharp
public Style Style { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FormatConditionPropertyStyleDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue(30);
            worksheet.Cells["A2"].PutValue(60);
            worksheet.Cells["A3"].PutValue(90);

            // إضافة تنسيق شرطي
            int index = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcs = worksheet.ConditionalFormattings[index];

            // تعيين النطاق
            CellArea area = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 0 };
            fcs.AddArea(area);

            // أضف الشرط الأول (القيم بين 40-80)
            int conditionIndex1 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.Between, "40", "80");
            FormatCondition fc1 = fcs[conditionIndex1];
            fc1.Style.BackgroundColor = System.Drawing.Color.Yellow;
            fc1.Style.Font.Color = System.Drawing.Color.Black;

            // أضف الشرط الثاني (القيم > 80)
            int conditionIndex2 = fcs.AddCondition(FormatConditionType.CellValue, OperatorType.GreaterThan, "80", null);
            FormatCondition fc2 = fcs[conditionIndex2];
            fc2.Style.BackgroundColor = System.Drawing.Color.Green;
            fc2.Style.Font.Color = System.Drawing.Color.White;
            fc2.Style.Font.IsBold = true;

            // احفظ المصنف
            workbook.Save("FormatConditionStyleDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Style](../../style/)
* class [FormatCondition](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


