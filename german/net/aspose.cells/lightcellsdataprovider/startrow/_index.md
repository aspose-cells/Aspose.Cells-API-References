---
title: "LightCellsDataProvider.StartRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LightCellsDataProvider-Methode. Beginnt mit dem Speichern von Daten einer Zeile"
type: docs
url: /de/net/aspose.cells/lightcellsdataprovider/startrow/
---
## LightCellsDataProvider.StartRow method

Beginnt, Daten einer Zeile zu speichern.

```csharp
public void StartRow(Row row)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| row | Row | Row-Objekt für die Implementierung zum Befüllen von Daten. Sein Zeilenindex ist der Rückgabewert des letzten Aufrufs von [`NextRow`](../nextrow/). Wenn die Zeile im inneren Zellenmodell initialisiert wurde, wird das vorhandene Row-Objekt verwendet. Andernfalls wird ein temporäres Row-Objekt für die Implementierung zum Befüllen von Daten verwendet. |

### Hinweise

Sie wird zu Beginn des Speicherns einer Zeile und ihrer Zellen-Daten aufgerufen. Wenn die aktuelle Zeile einige benutzerdefinierte Eigenschaften wie Höhe, Stil, ...etc. hat, sollte die Implementierung diese Eigenschaften hier im übergebenen Row-Objekt setzen.

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodStartRowWithRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle einen benutzerdefinierten Datenanbieter
            var saveOptions = new OoxmlSaveOptions
            {
                LightCellsDataProvider = new CustomLightCellsDataProvider()
            };

            try
            {
                // Verarbeite die Arbeitsmappe mit unserem benutzerdefinierten Datenanbieter
                workbook.Save("StartRowDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook processed successfully with StartRow implementation.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartRow method: {ex.Message}");
            }
        }

        private class CustomLightCellsDataProvider : LightCellsDataProvider
        {
            private int currentRow = -1;
            private readonly int totalRows = 5;

            public bool StartSheet(int sheetIndex)
            {
                return sheetIndex == 0;
            }

            public int NextRow()
            {
                currentRow++;
                return currentRow < totalRows ? currentRow : -1;
            }

            public void StartRow(Row row)
            {
                // Demonstriere die StartRow-Methode mit Row-Parameter
                row.Height = 25;
                row.IsHidden = (currentRow % 2 == 0);
                Console.WriteLine($"Processing row {row.Index}, Height: {row.Height}, Hidden: {row.IsHidden}");
            }

            public int NextCell()
            {
                return 0; // Process only first cell in each row
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue($"Row {cell.Row + 1} Data");
            }

            public bool IsGatherString()
            {
                return false;
            }
        }
    }
}
```

### Siehe auch

* class [Row](../../row/)
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


