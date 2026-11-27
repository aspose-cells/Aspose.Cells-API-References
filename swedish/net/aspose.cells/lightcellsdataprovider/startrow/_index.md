---
title: "LightCellsDataProvider.StartRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LightCellsDataProvider‑metod. Påbörjar att spara data för en rad"
type: docs
url: /sv/net/aspose.cells/lightcellsdataprovider/startrow/
---
## LightCellsDataProvider.StartRow method

Påbörjar sparandet av data för en rad.

```csharp
public void StartRow(Row row)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| row | Row | Rad‑objekt för implementering att fylla med data. Dess radindex är det returnerade värdet från det senaste anropet av [`NextRow`](../nextrow/). Om raden har initierats i den interna cellmodellen kommer det befintliga rad‑objektet att användas. Annars kommer ett temporärt Row‑objekt att användas för implementeringen att fylla med data. |

### Anmärkningar

Den kommer att anropas i början av att spara en rad och dess celldata. Om den aktuella raden har vissa anpassade egenskaper såsom höjd, stil, …etc., bör implementeringen sätta dessa egenskaper på det givna Row‑objektet här.

### Exempel

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
            
            // Skapa en anpassad dataleverantör
            var saveOptions = new OoxmlSaveOptions
            {
                LightCellsDataProvider = new CustomLightCellsDataProvider()
            };

            try
            {
                // Bearbeta arbetsboken med vår anpassade dataleverantör
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
                // Demonstrera StartRow‑metoden med Row‑parameter
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

### Se även

* class [Row](../../row/)
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


