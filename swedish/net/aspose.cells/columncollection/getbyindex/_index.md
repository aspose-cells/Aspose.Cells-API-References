---
title: "ColumnCollection.GetByIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ColumnCollection-metod. Hämtar kolumnobjektet efter indexet"
type: docs
url: /sv/net/aspose.cells/columncollection/getbyindex/
---
## ColumnCollection.GetByIndex method

Hämtar kolumnobjektet efter indexet.

```csharp
[Obsolete("Use Columns.GetColumnByIndex() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public Column GetByIndex(int index)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | Int32 |  |

### Returvärde

Returnerar kolumnobjektet.

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället Columns.GetColumnByIndex()-metoden. Denna egenskap kommer att tas bort 12 månader senare sedan juni 2010. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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

            // Skapa kolumner i samlingen genom att ange bredder
            worksheet.Cells.Columns[0].Width = 15;  // Column 0
            worksheet.Cells.Columns[2].Width = 20;  // Column 2
            worksheet.Cells.Columns[4].Width = 25;  // Column 4

            try
            {
                // Hämta andra kolumnen från ColumnCollection (index 1)
                Column column = worksheet.Cells.Columns.GetByIndex(1);

                Console.WriteLine($"Retrieved column at collection index 1");
                Console.WriteLine($"Worksheet column index: {column.Index}");
                Console.WriteLine($"Original width: {column.Width}");

                // Ändra den hämtade kolumnen
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

### Se även

* class [Column](../../column/)
* class [ColumnCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


