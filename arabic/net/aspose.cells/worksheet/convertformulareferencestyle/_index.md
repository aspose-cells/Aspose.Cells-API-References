---
title: "Worksheet.ConvertFormulaReferenceStyle"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Worksheet. تحول نمط إشارة الصيغة"
type: docs
url: /ar/net/aspose.cells/worksheet/convertformulareferencestyle/
---
## Worksheet.ConvertFormulaReferenceStyle method

يحوّل نمط مرجع الصيغة.

```csharp
public string ConvertFormulaReferenceStyle(string formula, bool toR1C1, int baseCellRow, 
    int baseCellColumn)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| صيغة | String | الصيغة التي سيتم تحويلها. |
| toR1C1 | منطقي | نمط الإشارة الذي سيتم تحويل الصيغة إليه. إذا كانت الصيغة الأصلية بنمط إشارة A1، يجب أن تكون هذه القيمة true بحيث يتم تحويل الصيغة من نمط A1 إلى R1C1؛ إذا كانت الصيغة الأصلية بنمط إشارة R1C1، يجب أن تكون هذه القيمة false بحيث يتم تحويل الصيغة من نمط R1C1 إلى A1؛ |
| baseCellRow | Int32 | فهرس الصف للخلية الأساسية. |
| baseCellColumn | Int32 | فهرس العمود للخلية الأساسية. |

### قيمة الإرجاع

الصيغة المحوّلة.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodConvertFormulaReferenceStyleWithStringBooleanInt32Int32Demo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];

            // مثال 1: تحويل نمط R1C1 إلى نمط A1
            string formulaR1C1 = "R[0]C23,testDS,R[0]C24";
            string formulaA1 = sheet.ConvertFormulaReferenceStyle(formulaR1C1, false, 0, 0);
            Console.WriteLine("Converted formula: " + formulaA1);

            // مثال 2: تحويل مع مراجع مختلطة
            string formulaMixed = "R[0]C23,testDS,rcurr,R[0]C24";
            string convertedMixed = sheet.ConvertFormulaReferenceStyle(formulaMixed, false, 0, 0);
            Console.WriteLine("Converted mixed formula: " + convertedMixed);
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


