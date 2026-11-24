---
title: "ColumnCollection.GetByIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ColumnCollection-Methode. Gibt das Spaltenobjekt anhand des Index zurück"
type: docs
url: /de/net/aspose.cells/columncollection/getbyindex/
---
## ColumnCollection.GetByIndex method

Gibt das Spaltenobjekt anhand des Index zurück.

```csharp
[Obsolete("Use Columns.GetColumnByIndex() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Column GetByIndex(int index)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | Int32 |  |

### Rückgabewert

Gibt das Spaltenobjekt zurück.

### Hinweise

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die Methode Columns.GetColumnByIndex(). Diese Eigenschaft wird 12 Monate nach Juni 2010 entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Ihnen entstanden sein könnten.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ColumnCollectionMethodGetByIndexWithInt32Demo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Spalten in der Sammlung durch Festlegen der Breiten erstellen
            worksheet.Cells.Columns[0].Width = 15;  // Column 0
            worksheet.Cells.Columns[2].Width = 20;  // Column 2
            worksheet.Cells.Columns[4].Width = 25;  // Column 4

            try
            {
                // Zweite Spalte aus ColumnCollection (Index 1) abrufen
                Column column = worksheet.Cells.Columns.GetByIndex(1);

                Console.WriteLine($"Retrieved column at collection index 1");
                Console.WriteLine($"Worksheet column index: {column.Index}");
                Console.WriteLine($"Original width: {column.Width}");

                // Die abgerufene Spalte ändern
                column.Width = 35;
                Console.WriteLine($"Updated width: {column.Width}");
            }
            catch (ArgumentOutOfRangeException ex)
            {
                Console.WriteLine($"Invalid index: {ex.Message}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ColumnCollectionGetByIndexDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


