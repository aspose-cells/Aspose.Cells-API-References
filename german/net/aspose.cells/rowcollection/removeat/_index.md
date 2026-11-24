---
title: "RowCollection.RemoveAt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "RowCollection-Methode. Entfernen Sie das Zeilenobjekt an der angegebenen Indexposition in dieser Sammlung"
type: docs
url: /de/net/aspose.cells/rowcollection/removeat/
---
## RowCollection.RemoveAt method

Entfernen Sie das Zeilenelement am angegebenen Index (Position) in dieser Sammlung.

```csharp
public void RemoveAt(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| index | Int32 | nullbasierter Index (Position, nicht [`Index`](../../row/index/)) des vorhandenen Zeilenobjekts in dieser Sammlung. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class RowCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie einigen Zellen in den ersten paar Zeilen Daten hinzu
            worksheet.Cells["A1"].PutValue("Row 1");
            worksheet.Cells["A2"].PutValue("Row 2");
            worksheet.Cells["A3"].PutValue("Row 3");
            worksheet.Cells["A4"].PutValue("Row 4");

            // Anfangszeilenanzahl anzeigen
            Console.WriteLine($"Initial row count: {worksheet.Cells.Rows.Count}");

            try
            {
                // Rufen Sie die RemoveAt-Methode auf, um die Zeile bei Index 1 (zweite Zeile) zu entfernen
                worksheet.Cells.Rows.RemoveAt(1);

                Console.WriteLine("Method executed successfully. Row at index 1 removed.");

                // Aktualisierte Zeilenanzahl anzeigen
                Console.WriteLine($"Updated row count: {worksheet.Cells.Rows.Count}");

                // Zeigen Sie den Effekt – Zeile 2 sollte entfernt werden, Zeile 3 wird zu Zeile 2
                Console.WriteLine("Cell A1: " + worksheet.Cells["A1"].StringValue);
                Console.WriteLine("Cell A2: " + worksheet.Cells["A2"].StringValue);
                Console.WriteLine("Cell A3: " + worksheet.Cells["A3"].StringValue);
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing RemoveAt method: {ex.Message}");
            }

            // Ergebnis speichern
            workbook.Save("RowCollectionMethodRemoveAtWithInt32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [RowCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


