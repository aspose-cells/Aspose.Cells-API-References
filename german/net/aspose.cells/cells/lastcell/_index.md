---
title: "Cells.LastCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Gibt die letzte Zelle in diesem Arbeitsblatt zurück"
type: docs
url: /de/net/aspose.cells/cells/lastcell/
---
## Cells.LastCell property

Ruft die letzte Zelle in diesem Arbeitsblatt ab.

```csharp
public Cell LastCell { get; }
```

### Hinweise

Gibt null zurück, wenn im Arbeitsblatt keine Daten vorhanden sind.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyLastCellDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Daten befüllen
            worksheet.Cells["A1"].Value = "Header1";
            worksheet.Cells["B1"].Value = "Header2";
            worksheet.Cells["A2"].Value = "Data1";
            worksheet.Cells["B2"].Value = "Data2";

            // Adresse der letzten Zelle abrufen
            Cell lastCell = worksheet.Cells.LastCell;
            Console.WriteLine("Last cell address: " + lastCell.Name);

            // Erstelle einen Bereich von der ersten bis zur letzten Zelle
            Aspose.Cells.Range fullRange = worksheet.Cells.CreateRange(
                worksheet.Cells.FirstCell.Name, 
                lastCell.Name);
            
            // Formatiere den Bereich
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            fullRange.ApplyStyle(style, new StyleFlag { FontBold = true });

            // Speichere die Arbeitsmappe
            workbook.Save("LastCellDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cell](../../cell/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


