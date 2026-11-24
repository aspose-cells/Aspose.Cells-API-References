---
title: "ListObject.HasAutoFilter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListObject-Eigenschaft. Gibt an, ob ein AutoFilter auf diese Tabelle angewendet wird"
type: docs
url: /de/net/aspose.cells.tables/listobject/hasautofilter/
---
## ListObject.HasAutoFilter property

Gibt an, ob der Auto-Filter auf diese Tabelle angewendet wird.

```csharp
public bool HasAutoFilter { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using System;
    using Aspose.Cells;
    using Aspose.Cells.Tables;

    public class ListObjectPropertyHasAutoFilterDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine neue Arbeitsmappe und rufen Sie das erste Arbeitsblatt ab
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten für die Tabelle füllen
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["A2"].PutValue("Alice");
            worksheet.Cells["B2"].PutValue(85);
            worksheet.Cells["A3"].PutValue("Bob");
            worksheet.Cells["B3"].PutValue(92);
            worksheet.Cells["A4"].PutValue("Charlie");
            worksheet.Cells["B4"].PutValue(78);

            try
            {
                // Ein ListObject (Tabelle) hinzufügen, das den Datenbereich abdeckt
                int tableIndex = worksheet.ListObjects.Add(0, 0, 3, 1, true);
                ListObject listObject = worksheet.ListObjects[tableIndex];

                // Sicherstellen, dass die Tabelle so angepasst wird, dass alle Zeilen enthalten sind
                listObject.Resize(0, 0, 4, 2, true);

                // Den Wert der HasAutoFilter-Eigenschaft lesen und anzeigen
                bool hasFilter = listObject.HasAutoFilter;
                Console.WriteLine("HasAutoFilter: " + hasFilter);

                // Auf das AutoFilter-Objekt kann über die AutoFilter-Eigenschaft zugegriffen werden
                // Demonstrieren, dass es nicht null ist, wenn HasAutoFilter wahr ist
                if (hasFilter && listObject.AutoFilter != null)
                {
                    // Einen einfachen Filter auf die Spalte "Score" (Index 1) anwenden, um Zeilen mit Score >= 80 anzuzeigen
                    listObject.AutoFilter.Filter(1, ">=80");

                    Console.WriteLine("Filtered rows (Score >= 80):");
                    for (int row = 1; row <= 4; row++)
                    {
                        // Verwenden Sie Cells.Rows, um zu prüfen, ob die Zeile ausgeblendet ist
                        if (!worksheet.Cells.Rows[row].IsHidden)
                        {
                            Console.WriteLine($"{worksheet.Cells[row, 0].StringValue} - {worksheet.Cells[row, 1].IntValue}");
                        }
                    }

                    // Filter zurücksetzen
                    listObject.AutoFilter.RemoveFilter(1);
                }

                // Arbeitsmappe speichern (optional)
                workbook.Save("HasAutoFilterDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Error: " + ex.Message);
            }
        }
    }
}
```

### Siehe auch

* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


