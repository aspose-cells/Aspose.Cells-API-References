---
title: "LightCellsDataProvider.NextCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LightCellsDataProvider‑metod. Hämtar nästa cell som ska sparas"
type: docs
url: /sv/net/aspose.cells/lightcellsdataprovider/nextcell/
---
## LightCellsDataProvider.NextCell method

Hämtar nästa cell som ska sparas.

```csharp
public int NextCell()
```

### Returvärde

kolumnindex för nästa cell som ska sparas. -1 betyder att slutet av den aktuella radens data har nåtts och ingen ytterligare cell i den aktuella raden ska sparas.

### Anmärkningar

Den kommer att anropas i början av att spara en cell.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodNextCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Clear();
            
            var provider = new DemoLightCellsDataProvider();
            XlsSaveOptions saveOptions = new XlsSaveOptions { LightCellsDataProvider = provider };

            try
            {
                workbook.Save("NextCellDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with LightCellsDataProvider implementation");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class DemoLightCellsDataProvider : LightCellsDataProvider
        {
            private int rowIndex = -1;
            private int cellIndex = -1;
            private readonly object[,] data = new object[2, 2]
            {
                { "Column1", "Column2" },
                { 100, 200 }
            };

            public bool StartSheet(int sheetIndex) => sheetIndex == 0;

            public int NextRow()
            {
                rowIndex++;
                cellIndex = -1;
                return rowIndex < 2 ? 1 : 0;
            }

            public void StartRow(Row row) { }

            public int NextCell()
            {
                cellIndex++;
                return cellIndex < 2 ? 1 : 0;
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue(data[rowIndex, cellIndex]);
            }

            public bool IsGatherString() => false;
        }
    }
}
```

### Se även

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


