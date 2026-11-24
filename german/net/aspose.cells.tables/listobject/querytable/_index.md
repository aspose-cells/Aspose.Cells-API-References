---
title: "ListObject.QueryTable"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ListObject-Eigenschaft. Gibt die verknüpfte QueryTable zurück"
type: docs
url: /de/net/aspose.cells.tables/listobject/querytable/
---
## ListObject.QueryTable property

Ermittelt die verknüpfte QueryTable.

```csharp
public QueryTable QueryTable { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class ListObjectPropertyQueryTableDemo
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
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Erstelle ein Listenobjekt
            int index = worksheet.ListObjects.Add(0, 0, 2, 1, true);
            ListObject listObject = worksheet.ListObjects[index];

            try
            {
                // Zugriff auf die QueryTable-Eigenschaft (schreibgeschützt)
                QueryTable queryTable = listObject.QueryTable;

                if (queryTable != null)
                {
                    // QueryTable-Eigenschaften anzeigen
                    Console.WriteLine("QueryTable Name: " + queryTable.Name);
                    Console.WriteLine("Connection ID: " + queryTable.ConnectionId);
                    Console.WriteLine("Preserve Formatting: " + queryTable.PreserveFormatting);
                    Console.WriteLine("Adjust Column Width: " + queryTable.AdjustColumnWidth);

                    // Zugriff auf den Ergebnisbereich, falls verfügbar
                    if (queryTable.ResultRange != null)
                    {
                        Console.WriteLine("Result Range Address: " + queryTable.ResultRange.Name);
                    }
                }
                else
                {
                    Console.WriteLine("No QueryTable associated with this ListObject");
                }

                // Speichere die Arbeitsmappe
                workbook.Save("QueryTableDemo.xlsx");
                Console.WriteLine("Workbook saved successfully.");
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

* class [QueryTable](../../../aspose.cells/querytable/)
* class [ListObject](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


