---
title: "LightCellsDataProvider.StartSheet"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LightCellsDataProvider‑metod. Påbörjar sparandet av ett kalkylblad"
type: docs
url: /sv/net/aspose.cells/lightcellsdataprovider/startsheet/
---
## LightCellsDataProvider.StartSheet method

Påbörjar sparandet av ett kalkylblad.

```csharp
public bool StartSheet(int sheetIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sheetIndex | Int32 | index för det aktuella kalkylbladet som ska sparas. |

### Returvärde

sant om denna leverantör kommer att tillhandahålla data för det angivna bladet; falskt om det angivna bladet ska använda sin vanliga datamodell (Cells).

### Anmärkningar

Den kommer att anropas i början av sparandet av ett kalkylblad under sparandet av en arbetsbok. Om leverantören behöver referera till

```csharp
sheetIndex
```

senare i startRow(Row)- eller startCell(Cell)-metoden, det vill säga om processen behöver veta vilket kalkylblad som bearbetas, bör implementationen behålla

```csharp
sheetIndex
```

värdet här.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodStartSheetWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                Workbook workbook = new Workbook();
                workbook.Worksheets.Clear(); // Start with clean worksheet
                
                // Skapa en anpassad dataleverantör och spara i lätta celler‑läge
                var saveOptions = new OoxmlSaveOptions
                {
                    LightCellsDataProvider = new CustomLightCellsDataProvider()
                };

                Console.WriteLine("Starting workbook save with LightCellsDataProvider...");
                workbook.Save("StartSheetDemoOutput.xlsx", saveOptions);
                Console.WriteLine("Workbook saved successfully. Check StartSheetDemoOutput.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing demo: {ex.Message}");
            }
        }

        private class CustomLightCellsDataProvider : LightCellsDataProvider
        {
            private bool sheetProcessed = false;

            // Anropas när ett kalkylblad ska bearbetas
            public bool StartSheet(int sheetIndex)
            {
                Console.WriteLine($"Processing sheet index: {sheetIndex}");
                // Bearbeta endast första bladet (index 0)
                if (sheetIndex == 0)
                {
                    sheetProcessed = true;
                    return true;
                }
                return false;
            }

            public int NextRow()
            {
                if (sheetProcessed)
                {
                    sheetProcessed = false;
                    return 0; // Process first row (index 0)
                }
                return -1; // Stop processing after first row
            }

            public void StartRow(Row row)
            {
                row.Height = 20;
            }

            public int NextCell()
            {
                return 0; // Process first cell (index 0)
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue("Data from LightCellsDataProvider");
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

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


