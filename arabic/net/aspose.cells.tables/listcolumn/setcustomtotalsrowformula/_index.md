---
title: "ListColumn.SetCustomTotalsRowFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ListColumn. تحصل على صيغة الصف الإجمالي لهذا العمود في القائمة"
type: docs
url: /ar/net/aspose.cells.tables/listcolumn/setcustomtotalsrowformula/
---
## ListColumn.SetCustomTotalsRowFormula method

يحصل على صيغة صف الإجماليات لهذا عمود القائمة.

```csharp
public void SetCustomTotalsRowFormula(string formula, bool isR1C1, bool isLocal)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صيغة | String | الصيغة لهذا العمود في القائمة. |
| isR1C1 | منطقي | ما إذا كان يجب تنسيق الصيغة كـ R1C1. |
| isLocal | منطقي | ما إذا كان يجب تنسيق الصيغة وفقًا للمنطقة. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListColumnMethodSetCustomTotalsRowFormulaWithStringBooleanBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("Column1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(20);

            // إنشاء كائن قائمة
            int index = worksheet.ListObjects.Add(0, 0, 2, 0, true);
            ListObject listObject = worksheet.ListObjects[index];

            // تمكين الصف الإجمالي وتعيين صيغة مخصصة
            listObject.ShowTotals = true;
            listObject.ListColumns[0].TotalsCalculation = TotalsCalculation.Custom;
            listObject.ListColumns[0].SetCustomTotalsRowFormula("=SUM([Column1])", false, false);

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


