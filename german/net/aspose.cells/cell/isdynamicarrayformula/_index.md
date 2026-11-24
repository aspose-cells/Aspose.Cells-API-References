---
title: "Cell.IsDynamicArrayFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Zellen-Eigenschaft. Gibt an, ob die Formel der Zelle eine dynamische Array-Formel (true) oder eine Legacy-Array-Formel (false) ist"
type: docs
url: /de/net/aspose.cells/cell/isdynamicarrayformula/
---
## Cell.IsDynamicArrayFormula property

Gibt an, ob die Formel der Zelle eine dynamische Array‑Formel (true) oder eine Legacy‑Array‑Formel (false) ist.

```csharp
public bool IsDynamicArrayFormula { get; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsDynamicArrayFormulaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Eine dynamische Array-Formel in Zelle A1 festlegen
            worksheet.Cells["A1"].SetDynamicArrayFormula("=B1:B3", new FormulaParseOptions(), false);
            
            // Überprüfen, ob die Zelle eine dynamische Array-Formel enthält
            Console.WriteLine("Is A1 a dynamic array formula? " + worksheet.Cells["A1"].IsDynamicArrayFormula);

            // Speichere die Arbeitsmappe
            string outputPath = "DynamicArrayFormulaDemo.xlsx";
            workbook.Save(outputPath, SaveFormat.Xlsx);

            Console.WriteLine("Workbook saved with dynamic array formula at: " + outputPath);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


