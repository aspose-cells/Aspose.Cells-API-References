---
title: "ListObject.AutoFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListObject property. Ruft den AutoFilter dieser Tabelle ab"
type: docs
url: /de/net/aspose.cells.tables/listobject/autofilter/
---
## ListObject.AutoFilter property

Liest den Auto-Filter dieser Tabelle.

```csharp
public AutoFilter AutoFilter { get; }
```

### Hinweise

Es funktioniert nur, wenn [`HasAutoFilter`](../hasautofilter/) false ist.

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class ListObjectPropertyAutoFilterDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Mary");
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["A4"].PutValue("Peter");
            worksheet.Cells["B4"].PutValue(35);

            // Ein ListObject erstellen
            int index = worksheet.ListObjects.Add(0, 0, 3, 1, true);
            ListObject listObject = worksheet.ListObjects[index];

            // Größe des ListObjects ändern, um alle Daten einzuschließen
            listObject.Resize(0, 0, 4, 2, true);

            // Zugriff auf und Demonstration der AutoFilter-Funktionalität
            if (listObject.AutoFilter != null)
            {
                // Filter auf die Spalte Alter (Spalte 2) anwenden
                listObject.AutoFilter.Filter(1, "25");
                
                // Gefilterte Daten anzeigen
                Console.WriteLine("Filtered Data:");
                for (int row = 1; row <= 4; row++)
                {
                    if (!worksheet.Cells.Rows[row].IsHidden)
                    {
                        Console.WriteLine($"{worksheet.Cells[row, 0].StringValue} - {worksheet.Cells[row, 1].IntValue}");
                    }
                }

                // Filter zurücksetzen
                listObject.AutoFilter.RemoveFilter(1);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("ListObjectAutoFilterDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [AutoFilter](../../../aspose.cells/autofilter/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


