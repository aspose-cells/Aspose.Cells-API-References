---
title: "Cell.IsFormula"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt an, ob die angegebene Zelle eine Formel enthält"
type: docs
url: /de/net/aspose.cells/cell/isformula/
---
## Cell.IsFormula property

Gibt an, ob die angegebene Zelle eine Formel enthält.

```csharp
public bool IsFormula { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIsFormulaDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Formel zu Zelle A1 hinzufügen
            worksheet.Cells["A1"].Formula = "=1+2";
            
            // Einfachen Wert zu Zelle A2 hinzufügen
            worksheet.Cells["A2"].PutValue("Test");
            
            // Prüfen, ob Zellen Formeln enthalten
            Console.WriteLine("A1 is formula: " + worksheet.Cells["A1"].IsFormula);
            Console.WriteLine("A2 is formula: " + worksheet.Cells["A2"].IsFormula);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


