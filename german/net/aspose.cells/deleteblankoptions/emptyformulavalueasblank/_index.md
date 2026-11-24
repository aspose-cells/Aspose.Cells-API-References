---
title: "DeleteBlankOptions.EmptyFormulaValueAsBlank"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DeleteBlankOptions-Eigenschaft. Ob eine Zelle als leer betrachtet wird, wenn sie eine Formel ist und das berechnete Ergebnis null oder ein leerer String ist. Standardwert ist false"
type: docs
url: /de/net/aspose.cells/deleteblankoptions/emptyformulavalueasblank/
---
## DeleteBlankOptions.EmptyFormulaValueAsBlank property

Ob eine Zelle als leer betrachtet wird, wenn sie eine Formel ist und das berechnete Ergebnis null oder ein leerer String ist. Standardwert ist false.

```csharp
public bool EmptyFormulaValueAsBlank { get; set; }
```

### Hinweise

Im Allgemeinen sollte der Benutzer sicherstellen, dass die Formeln berechnet wurden, bevor die Löschoperation mit dieser Eigenschaft auf true gesetzt wird. Andernfalls werden alle neu erstellten Formeln über normale APIs wie [`Formula`](../../cell/formula/) als leer betrachtet und können gelöscht werden, weil ihre berechneten Ergebnisse vor der Berechnung alle null sind.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEmptyFormulaValueAsBlankDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;

            // Beispieldaten befüllen
            cells["A1"].PutValue("Header");
            cells["A2"].Formula = "=B2";  // Formula returning blank
            cells["A3"].PutValue("Data");
            cells["A4"].Formula = "=1+1"; // Formula with value
            
            // Leere Zeilen löschen, ohne Formel-Leerwerte zu berücksichtigen
            Console.WriteLine("Before deletion (normal): " + cells.MaxRow + " rows");
            cells.DeleteBlankRows();
            Console.WriteLine("After normal deletion: " + cells.MaxRow + " rows");

            // Daten zurücksetzen
            cells.ClearContents(0, 0, cells.MaxRow + 1, cells.MaxColumn + 1);
            cells["A1"].PutValue("Header");
            cells["A2"].Formula = "=B2";
            cells["A3"].PutValue("Data");
            cells["A4"].Formula = "=1+1";

            // Leere Zeilen löschen, wobei Formel-Leerstellen als leer behandelt werden
            Console.WriteLine("\nBefore deletion (with EmptyFormulaValueAsBlank): " + cells.MaxRow + " rows");
            cells.DeleteBlankRows(new DeleteBlankOptions() { EmptyFormulaValueAsBlank = true });
            Console.WriteLine("After deletion with EmptyFormulaValueAsBlank: " + cells.MaxRow + " rows");
        }
    }
}
```

### Siehe auch

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


