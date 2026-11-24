---
title: "ColumnCollection.GetColumnByIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ColumnCollection-Methode. Ruft das Column-Objekt anhand seiner Position in der Liste ab"
type: docs
url: /de/net/aspose.cells/columncollection/getcolumnbyindex/
---
## ColumnCollection.GetColumnByIndex method

Ruft das [`Column`](../../column/)‑Objekt anhand seiner Position in der Liste ab.

```csharp
public Column GetColumnByIndex(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 | Die Position in der Liste. |

### Rückgabewert

Gibt das Spaltenobjekt zurück.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ColumnCollectionMethodGetColumnByIndexWithInt32Demo
    {
        public static void Run()
        {
            // Erstelle eine neue Arbeitsmappe und greife auf das erste Arbeitsblatt zu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten zu Spalte A hinzufügen
            worksheet.Cells["A1"].Value = "Aspose.Cells Column Demo";

            try
            {
                // Referenz zur Spaltensammlung abrufen
                ColumnCollection columns = worksheet.Cells.Columns;

                // Auf Spalte bei Index 0 (Spalte A) mit GetColumnByIndex zugreifen
                Column column = columns.GetColumnByIndex(0);

                // Spaltenbreite ändern, um den Spaltenzugriff zu demonstrieren
                column.Width = 25;

                Console.WriteLine("Modified width of column at index 0 (Column A) to 25 characters.");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid column index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            // Speichere die geänderte Arbeitsmappe
            workbook.Save("ColumnCollectionMethodGetColumnByIndexWithInt32Demo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


