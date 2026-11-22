---
title: "Cell.Calculate"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تحسب صيغة الخلية"
type: docs
url: /ar/net/aspose.cells/cell/calculate/
---
## Cell.Calculate method

يحسب صيغة الخلية.

```csharp
public void Calculate(CalculationOptions options)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| خيارات | CalculationOptions | خيارات الحساب |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodCalculateWithCalculationOptionsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تعيين صيغة بسيطة في الخلية A1
            Cell cellA1 = worksheet.Cells["A1"];
            cellA1.Formula = "=SUM(1, 2, 3)";
            
            // احسب باستخدام الخيارات الافتراضية
            cellA1.Calculate(new CalculationOptions());
            Console.WriteLine("A1 value after calculation: " + cellA1.Value);

            // تعيين صيغة مصفوفة في النطاق B1:D1
            Cell cellB1 = worksheet.Cells["B1"];
            cellB1.SetArrayFormula("={1,2,3}", 1, 3);
            
            // احسب صيغة المصفوفة باستخدام الخيارات
            cellB1.Calculate(new CalculationOptions());
            Console.WriteLine("B1 value after calculation: " + cellB1.Value);

            // تعيين صيغة أكثر تعقيدًا في الخلية A2
            Cell cellA2 = worksheet.Cells["A2"];
            cellA2.Formula = "=IF(A1>5, \"Greater\", \"Less or equal\")";
            
            // احسب باستخدام الخيارات
            cellA2.Calculate(new CalculationOptions());
            Console.WriteLine("A2 value after calculation: " + cellA2.Value);
        }
    }
}
```

### انظر أيضًا

* class [CalculationOptions](../../calculationoptions/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


