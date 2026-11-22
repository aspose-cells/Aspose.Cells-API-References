---
title: "ListColumn.GetCustomTotalsRowFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ListColumn. تحصل على صيغة الصف الإجمالي لهذا العمود في القائمة"
type: docs
url: /ar/net/aspose.cells.tables/listcolumn/getcustomtotalsrowformula/
---
## ListColumn.GetCustomTotalsRowFormula method

يحصل على صيغة صف الإجماليات لهذا عمود القائمة.

```csharp
public string GetCustomTotalsRowFormula(bool isR1C1, bool isLocal)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| isR1C1 | منطقي | ما إذا كان يجب تنسيق الصيغة كـ R1C1. |
| isLocal | منطقي | ما إذا كان يجب تنسيق الصيغة وفقًا للمنطقة. |

### قيمة الإرجاع

الصيغة لهذا العمود في القائمة.

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnMethodGetCustomTotalsRowFormulaWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);

            // إنشاء كائن قائمة
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            ListObject listObject = worksheet.ListObjects[index];

            // تعيين صيغة إجماليات مخصصة
            ListColumn listColumn = listObject.ListColumns[0];
            listColumn.TotalsCalculation = Aspose.Cells.Tables.TotalsCalculation.Custom;
            listColumn.SetCustomTotalsRowFormula("=SUM([Column1])", false, false);

            // احصل على صيغة الإجماليات المخصصة واعرضها
            string formula = listColumn.GetCustomTotalsRowFormula(false, true);
            Console.WriteLine("Custom Totals Formula: " + formula);

            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


