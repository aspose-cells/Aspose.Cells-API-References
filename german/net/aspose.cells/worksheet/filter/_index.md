---
title: "Worksheet.Filter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet‑Methode. Filtert den Bereich"
type: docs
url: /de/net/aspose.cells/worksheet/filter/
---
## Worksheet.Filter method

Filtert den Bereich.

```csharp
public void Filter(CellArea ca)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| ca | CellArea | Der Bereich |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;

    public class WorksheetMethodFilterWithCellAreaDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füllen Sie einige Beispieldaten ein (einschließlich einer Kopfzeile)
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(40);

            try
            {
                // Definieren Sie den Bereich, auf den der Filter angewendet wird
                CellArea filterArea = new CellArea
                {
                    StartRow = 0,      // Row 1 (zero‑based)
                    StartColumn = 0,   // Column A
                    EndRow = 4,        // Row 5
                    EndColumn = 1      // Column B
                };

                // Wenden Sie einen Auto‑Filter auf den definierten Bereich an
                worksheet.Filter(filterArea);

                // Speichern Sie die Arbeitsmappe, um zu überprüfen, ob der Filter gesetzt wurde
                workbook.Save("WorksheetFilterWithCellAreaDemo.xlsx");

                Console.WriteLine("Filter applied successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error applying filter: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* struct [CellArea](../../cellarea/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


