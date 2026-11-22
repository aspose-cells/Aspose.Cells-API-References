---
title: "Cell.GetArrayRange"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. يحصل على نطاق المصفوفة إذا كانت صيغة الخلية صيغة مصفوفة"
type: docs
url: /ar/net/aspose.cells/cell/getarrayrange/
---
## Cell.GetArrayRange method

يحصل على نطاق المصفوفة إذا كانت صيغة الخلية صيغة مصفوفة.

```csharp
public CellArea GetArrayRange()
```

### قيمة الإرجاع

نطاق المصفوفة.

### ملاحظات

يطبق فقط عندما تكون صيغة الخلية صيغة مصفوفة

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetArrayRangeDemo
    {
        public static void Run()
        {
            // إنشاء مصنف
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            
            // تعيين صيغة مصفوفة ديناميكية في الخلية A1
            Cell cell = cells[0, 0];
            string formula = "=SEQUENCE(3,2)";
            cell.SetDynamicArrayFormula(formula, new FormulaParseOptions(), false);
            
            // حساب الصيغ
            wb.CalculateFormula();
            
            // احصل على نطاق المصفوفة للصيغة الديناميكية
            CellArea arrayRange = cell.GetArrayRange();
            
            // إخراج معلومات نطاق المصفوفة
            Console.WriteLine("Array range for dynamic formula:");
            Console.WriteLine($"Start row: {arrayRange.StartRow}");
            Console.WriteLine($"Start column: {arrayRange.StartColumn}");
            Console.WriteLine($"End row: {arrayRange.EndRow}");
            Console.WriteLine($"End column: {arrayRange.EndColumn}");
            
            // طباعة القيم في نطاق المصفوفة
            Console.WriteLine("\nValues in the array range:");
            for (int r = arrayRange.StartRow; r <= arrayRange.EndRow; r++)
            {
                for (int c = arrayRange.StartColumn; c <= arrayRange.EndColumn; c++)
                {
                    Console.Write(cells[r, c].Value + "\t");
                }
                Console.WriteLine();
            }
        }
    }
}
```

### انظر أيضًا

* struct [CellArea](../../cellarea/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


