---
title: "Cell.BoolValue"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cell-Eigenschaft. Gibt den booleschen Wert zurück, der in der Zelle enthalten ist"
type: docs
url: /de/net/aspose.cells/cell/boolvalue/
---
## Cell.BoolValue property

Liefert den booleschen Wert, der in der Zelle enthalten ist.

```csharp
public bool BoolValue { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyBoolValueDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Cell cell = cells[0, 0];
            
            // Legen Sie eine Formel fest, die zu einem booleschen Wert evaluiert
            cell.Formula = "=2.01>2";
            
            // Berechnen Sie die Formel, um das Ergebnis zu erhalten
            workbook.CalculateFormula();
            
            // Demonstrieren Sie die BoolValue-Eigenschaft
            Console.WriteLine("Cell BoolValue: " + cell.BoolValue);
        }
    }
}
```

### Siehe auch

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


