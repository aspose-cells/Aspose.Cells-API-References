---
title: "FilterColumn.Top10Filter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FilterColumn-Eigenschaft. Liefert Top10Filter zum Filtern von Daten nach Rang der Daten"
type: docs
url: /de/net/aspose.cells/filtercolumn/top10filter/
---
## FilterColumn.Top10Filter property

Liefert `Top10Filter` zum Filtern von Daten nach Rang der Daten.

```csharp
public Top10Filter Top10Filter { get; }
```

### Hinweise

Bevor Sie diese Eigenschaft verwenden, stellen Sie bitte sicher, dass [`FilterType`](../filtertype/) Top10 ist, andernfalls wird null zurückgegeben.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FilterColumnPropertyTop10FilterDemo
    {
        public static void Run()
        {
            try
            {
                // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
                Workbook workbook = new Workbook();
                Worksheet sheet = workbook.Worksheets[0];

                // Einige Beispieldaten einfügen
                sheet.Cells["A1"].PutValue("Values");
                sheet.Cells["A2"].PutValue(10);
                sheet.Cells["A3"].PutValue(20);
                sheet.Cells["A4"].PutValue(30);
                sheet.Cells["A5"].PutValue(40);

                // Wenden Sie einen AutoFilter auf den Datenbereich an
                sheet.AutoFilter.Range = "A1:A5";

                // Ermitteln Sie die erste Filterspalte (Spaltenindex 0)
                FilterColumn filterColumn = sheet.AutoFilter.FilterColumns[0];

                // Zeigen Sie das aktuelle Filter-Objekt an (kann null sein)
                Console.WriteLine("Current Filter object type: " +
                    (filterColumn.Filter != null ? filterColumn.Filter.GetType().FullName : "null"));

                // Überprüfen Sie, ob der angewendete Filter ein Top10Filter ist
                if (filterColumn.Filter != null && filterColumn.Filter.GetType().Name == "Top10Filter")
                {
                    Console.WriteLine("The filter column contains a Top10Filter.");
                }
                else
                {
                    Console.WriteLine("No Top10Filter is applied to this column.");
                }

                // Arbeitsmappe speichern (optional)
                workbook.Save("Top10FilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Siehe auch

* class [Top10Filter](../../top10filter/)
* class [FilterColumn](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


