---
title: "FindOptions.SearchOrderByRows"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FindOptions‑Eigenschaft. Gibt an, ob die Suchreihenfolge nach Zeilen oder Spalten erfolgt"
type: docs
url: /de/net/aspose.cells/findoptions/searchorderbyrows/
---
## FindOptions.SearchOrderByRows property

Gibt an, ob die Suchreihenfolge nach Zeilen oder Spalten erfolgt.

```csharp
public bool SearchOrderByRows { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertySearchOrderByRowsDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe und füge Beispieldaten hinzu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füllen Sie Zellen mit Testdaten (Suche nach "abc" in spaltenbasierter Reihenfolge)
            worksheet.Cells["A1"].PutValue("xyz");
            worksheet.Cells["B1"].PutValue("def");
            worksheet.Cells["A2"].PutValue("123");
            worksheet.Cells["B2"].PutValue("abc");
            worksheet.Cells["A3"].PutValue("abc");
            worksheet.Cells["B3"].PutValue("789");

            // Erstellen Sie FindOptions und setzen Sie die Suchreihenfolge auf spaltenbasiert
            FindOptions findOptions = new FindOptions();
            findOptions.SearchOrderByRows = false; // Search column by column

            // Suche "abc" – sollte A3 (Zeile 2, Spalte 0) zurückgeben, wenn spaltenbasiert gesucht wird
            Cell foundCell = worksheet.Cells.Find("abc", null, findOptions);

            // Gib das Ergebnis aus
            Console.WriteLine($"Found 'abc' at row: {foundCell.Row}, column: {foundCell.Column}");
        }
    }
}
```

### Siehe auch

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


