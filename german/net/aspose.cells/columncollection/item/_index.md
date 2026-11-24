---
title: "ColumnCollection.Item"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ColumnCollection-Eigenschaft. Gibt ein Column-Objekt anhand des Spaltenindex zurück. Das Column-Objekt des angegebenen Spaltenindex wird erstellt, falls es vorher nicht existiert."
type: docs
url: /de/net/aspose.cells/columncollection/item/
---
## ColumnCollection indexer

Ruft ein [`Column`](../../column/) Objekt anhand des Spaltenindex ab. Das Column-Objekt des angegebenen Spaltenindex wird erstellt, falls es vorher nicht existiert.

```csharp
public Column this[int columnIndex] { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ColumnCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Zugriff auf die Spaltensammlung
            ColumnCollection columns = worksheet.Cells.Columns;
            
            // Breite für Spalten über die Item-Eigenschaft festlegen
            columns[0].Width = 10;
            columns[1].Width = 15;
            columns[2].Width = 20;
            
            // Spaltenbreiten anzeigen
            Console.WriteLine("Column 0 Width: " + columns[0].Width);
            Console.WriteLine("Column 1 Width: " + columns[1].Width);
            Console.WriteLine("Column 2 Width: " + columns[2].Width);
            
            // Überprüfen, ob die Spaltenbreiten korrekt gesetzt sind
            if (columns[0].Width != 10 || columns[1].Width != 15 || columns[2].Width != 20)
            {
                throw new Exception("Column widths were not set correctly");
            }
        }
    }
}
```

### Siehe auch

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


