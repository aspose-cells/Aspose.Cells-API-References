---
title: "Cell.IsArrayFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt an, ob die Zellformel eine Array-Formel ist"
type: docs
url: /de/net/aspose.cells/cell/isarrayformula/
---
## Cell.IsArrayFormula property

Gibt an, ob die Zellenformel eine Array‑Formel ist.

```csharp
public bool IsArrayFormula { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsArrayFormulaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstellen Sie eine Array-Formel in Zelle B2
            worksheet.Cells["B2"].SetArrayFormula("SUM(A1:A10*B1:B10)", 1, 1);
            
            // Überprüfen Sie, ob die Zelle eine Array-Formel enthält
            bool isArrayFormula = worksheet.Cells["B2"].IsArrayFormula;
            
            // Gib das Ergebnis aus
            Console.WriteLine("Cell B2 is an array formula: " + isArrayFormula);
            
            // Speichere die Arbeitsmappe
            workbook.Save("IsArrayFormulaDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


