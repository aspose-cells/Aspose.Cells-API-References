---
title: "LightCellsDataProvider.IsGatherString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LightCellsDataProvider‑metod. Kontrollerar om det aktuella strängvärdet i cellen behöver samlas in i en global pool"
type: docs
url: /sv/net/aspose.cells/lightcellsdataprovider/isgatherstring/
---
## LightCellsDataProvider.IsGatherString method

Kontrollerar om det aktuella strängvärdet i cellen behöver samlas in i en global pool.

```csharp
public bool IsGatherString()
```

### Returvärde

sant om strängvärdet behöver samlas in i en global pool för den resulterande filen.

### Anmärkningar

Insamling av strängvärden ger fördelar endast när det finns många duplicerade strängvärden för de celler som tillhandahålls av denna implementation. I detta fall sparar insamling av strängar mycket minne och genererar en mindre resulterande fil. Om det finns många strängvärden för cellerna som tillhandahålls av LightCellsDataProvider men få av dem är lika, kommer insamling av strängar att kräva mer minne och tid och ger ingen fördel för den resulterande filen.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodIsGatherStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Clear();
            
            var saveOptions = new OoxmlSaveOptions
            {
                LightCellsDataProvider = new CustomLightCellsDataProvider()
            };

            try
            {
                workbook.Save("IsGatherStringDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with IsGatherString implementation");
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
            private readonly object[,] data = new object[3, 2]
            {
                { "Product", "Price" },
                { "Laptop", 1200.50 },
                { "Phone", 899.99 }
            };

            public bool StartSheet(int sheetIndex)
            {
                return sheetIndex == 0;
            }

            public int NextRow()
            {
                rowIndex++;
                cellIndex = -1;
                return rowIndex < 3 ? rowIndex : -1;
            }

            public void StartRow(Row row)
            {
                row.Height = 15;
            }

            public int NextCell()
            {
                cellIndex++;
                return cellIndex < 2 ? cellIndex : -1;
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue(data[rowIndex, cellIndex]);
            }

            public bool IsGatherString()
            {
                // Samla endast strängar för rubrikraden (rowIndex 0)
                return rowIndex == 0;
            }
        }
    }
}
```

### Se även

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


