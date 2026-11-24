---
title: "Cells.CheckColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt das Column-Element oder null am angegebenen Spaltenindex zurück"
type: docs
url: /de/net/aspose.cells/cells/checkcolumn/
---
## Cells.CheckColumn method

Gibt das [`Column`](../../column/) Element oder null am angegebenen Spaltenindex zurück.

```csharp
public Column CheckColumn(int columnIndex)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| columnIndex | Int32 | Der Spaltenindex. |

### Rückgabewert

Das Column-Objekt.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodCheckColumnWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Setze einen Wert in Spalte 1 (B3)
            cells["B3"].PutValue("Sample Data");
            
            // Spalte 4 prüfen (E-Spalte)
            Column column = cells.CheckColumn(4);
            
            // Spalteneigenschaften ausgeben
            Console.WriteLine("Column Width: " + column.Width);
            Console.WriteLine("Column Index: " + column.Index);
        }
    }
}
```

### Siehe auch

* class [Column](../../column/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


