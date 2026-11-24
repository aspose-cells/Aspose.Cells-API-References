---
title: "Cell.IntValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell‑Eigenschaft. Gibt den im Feld enthaltenen Ganzzahlwert zurück"
type: docs
url: /de/net/aspose.cells/cell/intvalue/
---
## Cell.IntValue property

Liefert den ganzzahligen Wert, der in der Zelle enthalten ist.

```csharp
public int IntValue { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyIntValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Setze einen numerischen Wert und rufe IntValue ab
            Cell cell1 = cells[0, 0];
            cell1.PutValue(42);
            Console.WriteLine("IntValue of numeric cell: " + cell1.IntValue);

            // Setze eine Formel, die zu einer Zahl auswertet, und rufe IntValue ab
            Cell cell2 = cells[0, 1];
            cell2.Formula = "=10+5";
            workbook.CalculateFormula();
            Console.WriteLine("IntValue of formula cell: " + cell2.IntValue);

            // Setze einen booleschen Wert und rufe IntValue ab
            Cell cell3 = cells[0, 2];
            cell3.PutValue(true);
            Console.WriteLine("IntValue of boolean cell: " + cell3.IntValue);

            // Setze einen Textwert und rufe IntValue ab (wird 0 sein, wenn nicht konvertierbar)
            Cell cell4 = cells[0, 3];
            cell4.PutValue("Hello");
            Console.WriteLine("IntValue of text cell: " + cell4.IntValue);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


