---
title: "LightCellsDataProvider.NextRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LightCellsDataProvider‑metod. Hämtar nästa rad som ska sparas"
type: docs
url: /sv/net/aspose.cells/lightcellsdataprovider/nextrow/
---
## LightCellsDataProvider.NextRow method

Hämtar nästa rad som ska sparas.

```csharp
public int NextRow()
```

### Returvärde

nästa radindex att sparas. -1 betyder att slutet av det aktuella bladets data har nåtts och ingen ytterligare rad i det aktuella bladet ska sparas.

### Anmärkningar

Den kommer att anropas i början av att spara en rad och dess celldata (innan [`StartRow`](../startrow/)).

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodNextRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Clear();
            workbook.Worksheets.Add("Sheet1");

            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();

            try
            {
                workbook.Save("LightCellsDataProviderMethodNextRowDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with LightCellsDataProvider implementation.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        private int currentRow = -1;
        private int currentCell = -1;
        private readonly int totalRows = 3;

        public bool StartSheet(int sheetIndex)
        {
            return sheetIndex == 0;
        }

        public int NextRow()
        {
            currentRow++;
            currentCell = -1;
            return currentRow < totalRows ? currentRow : -1;
        }

        public void StartRow(Row row)
        {
            row.Height = 20;
        }

        public int NextCell()
        {
            currentCell++;
            return currentCell < 2 ? currentCell : -1;
        }

        public void StartCell(Cell cell)
        {
            cell.PutValue($"R{currentRow}C{currentCell}");
        }

        public bool IsGatherString()
        {
            return false;
        }
    }
}
```

### Se även

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


