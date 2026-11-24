---
title: "Cell.IsSharedFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell‑Eigenschaft. Gibt an, ob die Zellformel Teil einer gemeinsam genutzten Formel ist"
type: docs
url: /de/net/aspose.cells/cell/issharedformula/
---
## Cell.IsSharedFormula property

Gibt an, ob die Zellformel Teil einer gemeinsamen Formel ist.

```csharp
public bool IsSharedFormula { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsSharedFormulaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Setze eine gemeinsam genutzte Formel in einem Bereich
            worksheet.Cells["B2"].Formula = "=A2*2";
            worksheet.Cells["B2"].Copy(worksheet.Cells["B3:B5"]);

            // Prüfe, ob Zellen eine gemeinsam genutzte Formel enthalten
            Cell cellB2 = worksheet.Cells["B2"];
            Cell cellB3 = worksheet.Cells["B3"];

            Console.WriteLine("Cell B2 IsSharedFormula: " + cellB2.IsSharedFormula);
            Console.WriteLine("Cell B3 IsSharedFormula: " + cellB3.IsSharedFormula);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


