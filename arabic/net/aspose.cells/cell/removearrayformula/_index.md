---
title: "Cell.RemoveArrayFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. إزالة صيغة المصفوفة"
type: docs
url: /ar/net/aspose.cells/cell/removearrayformula/
---
## Cell.RemoveArrayFormula method

إزالة صيغة المصفوفة.

```csharp
public void RemoveArrayFormula(bool leaveNormalFormula)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| leaveNormalFormula | منطقي | True تمثل تحويل صيغة المصفوفة إلى صيغة عادية. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodRemoveArrayFormulaWithBooleanDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // تعيين صيغة المصفوفة في خلية واحدة
            Cell cell = cells["A1"];
            cell.SetArrayFormula("=B1:D1", 1, 1);
            cells["B1"].PutValue(10);
            cells["C1"].PutValue(20);
            cells["D1"].PutValue(30);
            wb.CalculateFormula();

            Console.WriteLine("Before RemoveArrayFormula(false):");
            Console.WriteLine("IsArrayFormula: " + cell.IsArrayFormula);
            Console.WriteLine("Value: " + cell.Value);

            cell.RemoveArrayFormula(false);
            Console.WriteLine("\nAfter RemoveArrayFormula(false):");
            Console.WriteLine("IsFormula: " + cell.IsFormula);
            Console.WriteLine("Value: " + cell.Value);

            // تعيين صيغة المصفوفة مرة أخرى وإزالتها باستخدام معامل true
            cell.SetArrayFormula("=B1:D1", 1, 1);
            cell.RemoveArrayFormula(true);
            Console.WriteLine("\nAfter RemoveArrayFormula(true):");
            Console.WriteLine("IsArrayHeader: " + cell.IsArrayHeader);
            Console.WriteLine("Formula: " + cell.Formula);

            // تعيين صيغة المصفوفة عبر خلايا متعددة
            cell = cells["A1"];
            cell.SetArrayFormula("=B1:D1", 1, 3);
            cell.RemoveArrayFormula(false);
            Console.WriteLine("\nAfter multi-cell RemoveArrayFormula(false):");
            for (int i = 0; i < 3; i++)
            {
                Console.WriteLine($"Cell {cells[0, i].Name}: Value = {cells[0, i].Value}");
            }

            // تعيين صيغة المصفوفة مرة أخرى وإزالتها باستخدام معامل true
            cell.SetArrayFormula("=B1:D1", 1, 3);
            cell.RemoveArrayFormula(true);
            Console.WriteLine("\nAfter multi-cell RemoveArrayFormula(true):");
            for (int i = 0; i < 3; i++)
            {
                Console.WriteLine($"Cell {cells[0, i].Name}: Formula = {cells[0, i].Formula}");
            }
        }
    }
}
```

### انظر أيضًا

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


