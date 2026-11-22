---
title: "تعداد PivotTableAutoFormatType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Pivot.PivotTableAutoFormatType تعداد. يمثل نوع التنسيق التلقائي لجدول PivotTable."
type: docs
url: /ar/net/aspose.cells.pivot/pivottableautoformattype/
---
## PivotTableAutoFormatType enumeration

يمثل نوع التنسيق التلقائي لجدول PivotTable.

```csharp
public enum PivotTableAutoFormatType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | يمثل نوع التنسيق None. |
| Classic | `1` | يمثل نوع التنسيق التلقائي Classic. |
| Report1 | `2` | يمثل نوع التنسيق Report1. |
| Report2 | `3` | يمثل نوع التنسيق Report2. |
| Report3 | `4` | يمثل نوع التنسيق Report3. |
| Report4 | `5` | يمثل نوع التنسيق Report4. |
| Report5 | `6` | يمثل نوع التنسيق Report5. |
| Report6 | `7` | يمثل نوع التنسيق Report6. |
| Report7 | `8` | يمثل نوع التنسيق Report7. |
| Report8 | `9` | يمثل نوع التنسيق Report8. |
| Report9 | `10` | يمثل نوع التنسيق Report9. |
| Report10 | `11` | يمثل نوع التنسيق Report10. |
| Table1 | `12` | يمثل نوع التنسيق Table1. |
| Table2 | `13` | يمثل نوع تنسيق Table2. |
| Table3 | `14` | يمثل نوع تنسيق Table3. |
| Table4 | `15` | يمثل نوع تنسيق Table4. |
| Table5 | `16` | يمثل نوع تنسيق Table5. |
| Table6 | `17` | يمثل نوع تنسيق Table6. |
| Table7 | `18` | يمثل نوع تنسيق Table7. |
| Table8 | `19` | يمثل نوع تنسيق Table8. |
| Table9 | `20` | يمثل نوع تنسيق Table9. |
| Table10 | `21` | يمثل نوع تنسيق Table10. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableAutoFormatTypeDemo
    {
        public static void PivotTableAutoFormatTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بعض البيانات النموذجية إلى PivotTable
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 0].Value = "Apple";
            worksheet.Cells[3, 1].Value = 2021;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 0].Value = "Banana";
            worksheet.Cells[4, 1].Value = 2021;
            worksheet.Cells[4, 2].Value = 80;

            // إضافة PivotTable إلى ورقة العمل
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // إضافة حقول إلى PivotTable
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // حدد نوع التنسيق التلقائي لـ PivotTable
            pivotTable.AutoFormatType = PivotTableAutoFormatType.Report1;

            // احفظ المصنف
            workbook.Save("PivotTableAutoFormatTypeExample.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


