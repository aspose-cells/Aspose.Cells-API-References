---
title: "Cell.Row"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt die Zeilennummer (nullbasiert) der Zelle zurück"
type: docs
url: /de/net/aspose.cells/cell/row/
---
## Cell.Row property

Ermittelt die Zeilennummer (nullbasiert) der Zelle.

```csharp
public int Row { get; }
```

### Property Value

Cell-Zeilennummer

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieldaten und Formel hinzufügen
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");
            
            // Zelle mit Formel finden
            Cell cell = worksheet.Cells.Find("=SUM(A1", null, new FindOptions()
            { 
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.Contains 
            });
            
            // Demonstriere die Row-Eigenschaft.
            Console.WriteLine("Formula found in row: " + cell.Row);
            Console.WriteLine("Formula found in column: " + cell.Column);
            
            // Überprüfen Sie, ob die Zeile korrekt ist
            if (cell.Row == 2 && cell.Column == 0)
            {
                Console.WriteLine("Row property works correctly");
            }
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


