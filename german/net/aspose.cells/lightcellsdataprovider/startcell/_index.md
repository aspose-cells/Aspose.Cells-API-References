---
title: "LightCellsDataProvider.StartCell"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LightCellsDataProvider-Methode. Beginnt mit dem Speichern von Daten einer Zelle"
type: docs
url: /de/net/aspose.cells/lightcellsdataprovider/startcell/
---
## LightCellsDataProvider.StartCell method

Beginnt, Daten einer Zelle zu speichern.

```csharp
public void StartCell(Cell cell)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| cell | Cell | Cell-Objekt für die Implementierung zum Befüllen von Daten. Sein Spaltenindex ist der Rückgabewert des letzten Aufrufs von [`NextCell`](../nextcell/). Wenn die Zelle im inneren Zellenmodell initialisiert wurde, wird das vorhandene Cell-Objekt verwendet. Andernfalls wird ein temporäres Cell-Objekt für die Implementierung zum Befüllen von Daten verwendet. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodStartCellWithCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle eine Zelle, die als Parameter verwendet wird
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Data");
            
            // Erstelle einen benutzerdefinierten Datenanbieter
            var saveOptions = new OoxmlSaveOptions
            {
                LightCellsDataProvider = new CustomLightCellsDataProvider()
            };

            try
            {
                workbook.Save("StartCellWithCellDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with StartCell implementation");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class CustomLightCellsDataProvider : LightCellsDataProvider
        {
            private int rowIndex = -1;
            private int cellIndex = -1;
            private readonly int totalRows = 5;
            private readonly int totalCells = 3;

            public bool StartSheet(int sheetIndex)
            {
                return sheetIndex == 0;
            }

            public int NextRow()
            {
                rowIndex++;
                cellIndex = -1;
                return rowIndex < totalRows ? rowIndex : -1;
            }

            public void StartRow(Row row)
            {
                row.Height = 15;
            }

            public int NextCell()
            {
                cellIndex++;
                return cellIndex < totalCells ? cellIndex : -1;
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue($"Row {cell.Row + 1}, Col {cell.Column + 1}");
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

* class [Cell](../../cell/)
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


