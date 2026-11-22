---
title: "ListColumn.GetCustomCalculatedFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ListColumn. تحصل على صيغة هذا العمود في القائمة"
type: docs
url: /ar/net/aspose.cells.tables/listcolumn/getcustomcalculatedformula/
---
## ListColumn.GetCustomCalculatedFormula method

يحصل على الصيغة لهذا عمود القائمة.

```csharp
public string GetCustomCalculatedFormula(bool isR1C1, bool isLocal)
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
    public class ListColumnMethodGetCustomCalculatedFormulaWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // إنشاء بيانات نموذجية
            sheet.Cells["A1"].PutValue("Name");
            sheet.Cells["A2"].PutValue("John");
            sheet.Cells["A3"].PutValue("Mary");
            sheet.Cells["B1"].PutValue("Score");
            sheet.Cells["B2"].PutValue(85);
            sheet.Cells["B3"].PutValue(92);
            
            // إنشاء كائن قائمة
            int index = sheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = sheet.ListObjects[index];
            
            // أضف عمودًا محسوبًا
            ListColumn calcColumn = listObject.ListColumns[1];
            calcColumn.Formula = "=WEEKNUM([@Score])";
            
            // احصل على الصيغة المحسوبة المخصصة
            string formula = listObject.ListColumns[1].GetCustomCalculatedFormula(false, false);
            
            // أخرج النتيجة.
            Console.WriteLine("Calculated Formula: " + formula);
        }
    }
}
```

### انظر أيضًا

* class [ListColumn](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


