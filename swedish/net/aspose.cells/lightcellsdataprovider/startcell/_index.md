---
title: "LightCellsDataProvider.StartCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LightCellsDataProvider‑metod. Påbörjar att spara data för en cell"
type: docs
url: /sv/net/aspose.cells/lightcellsdataprovider/startcell/
---
## LightCellsDataProvider.StartCell method

Påbörjar sparandet av data för en cell.

```csharp
public void StartCell(Cell cell)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cell | Cell | Cell‑objekt för implementering att fylla med data. Dess kolumnindex är det returnerade värdet från det senaste anropet av [`NextCell`](../nextcell/). Om cellen har initierats i den interna cellmodellen kommer det befintliga cell‑objektet att användas. Annars kommer ett temporärt Cell‑objekt att användas för implementeringen att fylla med data. |

### Exempel

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
            
            // Skapa en cell att använda som parameter
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Data");
            
            // Skapa en anpassad dataleverantör
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

### Se även

* class [Cell](../../cell/)
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


