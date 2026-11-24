---
title: "Cells.MaxDisplayRange"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Gibt den maximalen Bereich zurück, der Daten, zusammengeführte Zellen und Formen enthält."
type: docs
url: /de/net/aspose.cells/cells/maxdisplayrange/
---
## Cells.MaxDisplayRange property

Ruft den maximalen Bereich ab, der Daten, zusammengeführte Zellen und Formen enthält.

```csharp
public Range MaxDisplayRange { get; }
```

### Hinweise

Gibt null zurück, wenn das Arbeitsblatt leer ist, seit Aspose.Cells 21.5.2.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxDisplayRangeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einige Daten zu Zellen hinzu, um einen Anzeigebereich zu erstellen
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["B2"].PutValue(200);
            worksheet.Cells["A3"].PutValue(300);
            worksheet.Cells["B3"].PutValue(400);

            // Den maximalen Anzeigebereich abrufen
            Aspose.Cells.Range maxDisplayRange = worksheet.Cells.MaxDisplayRange;

            // Gib die Bereichsinformationen aus
            Console.WriteLine("Max Display Range:");
            Console.WriteLine($"Start Row: {maxDisplayRange.FirstRow}");
            Console.WriteLine($"Start Column: {maxDisplayRange.FirstColumn}");
            Console.WriteLine($"Total Rows: {maxDisplayRange.RowCount}");
            Console.WriteLine($"Total Columns: {maxDisplayRange.ColumnCount}");

            // Erstelle einen neuen Bereich basierend auf den Abmessungen des maximalen Anzeigebereichs
            Aspose.Cells.Range customRange = worksheet.Cells.CreateRange(
                maxDisplayRange.FirstRow,
                maxDisplayRange.FirstColumn,
                maxDisplayRange.RowCount,
                maxDisplayRange.ColumnCount);

            // Formatiere den Bereich
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.LightGray;
            style.Pattern = BackgroundType.Solid;
            customRange.ApplyStyle(style, new StyleFlag { FontBold = true, CellShading = true });

            // Speichere die Arbeitsmappe
            workbook.Save("MaxDisplayRangeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../../range/)
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


