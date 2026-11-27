---
title: "LightCellsDataHandler.StartCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LightCellsDataHandler‑metod. Förbereder att bearbeta en cell"
type: docs
url: /sv/net/aspose.cells/lightcellsdatahandler/startcell/
---
## LightCellsDataHandler.StartCell method

Förbereder bearbetning av en cell.

```csharp
public bool StartCell(int columnIndex)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| columnIndex | Int32 | kolumnindex för cellen som ska bearbetas |

### Returvärde

om den här cellen behöver bearbetas. false för att ignorera cellen och kontrollera nästa tills slutet av celldata i den aktuella raden nås

### Anmärkningar

Den kommer att anropas när en befintlig cell i den aktuella raden nås. Aktuell rad är raden för det senaste anropet av [`ProcessRow`](../processrow/).

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LightCellsDataHandlerMethodStartCellWithInt32Demo
    {
        public static void Run()
        {
            try
            {
                // Skapa en tillfällig indatafil
                File.WriteAllText("input.csv", "Column1,Column2,Column3\n1,2,3\n4,5,6");

                // Skapa laddningsalternativ med anpassad LightCells-hanterare
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                var handler = new CustomLightCellsDataHandler();
                loadOptions.LightCellsDataHandler = handler;

                // Läs in arbetsbok med anpassad hanterare
                Workbook workbook = new Workbook("input.csv", loadOptions);

                // Spara den bearbetade arbetsboken
                workbook.Save("output.xlsx");
                Console.WriteLine("StartCell method executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing StartCell method: {ex.Message}");
            }
        }

        private class CustomLightCellsDataHandler : LightCellsDataHandler
        {
            public bool StartSheet(Worksheet sheet)
            {
                return true; // Process all sheets
            }

            public bool StartRow(int rowIndex)
            {
                return true; // Process all rows
            }

            public bool StartCell(int columnIndex)
            {
                // Bearbeta endast celler i kolumnindex 1 (andra kolumnen)
                return columnIndex == 1;
            }

            public bool ProcessCell(Cell cell)
            {
                // Dubbla värdet på cellerna i den andra kolumnen
                if (cell.IsNumericValue)
                {
                    cell.PutValue(cell.DoubleValue * 2);
                }
                return true;
            }

            public bool ProcessRow(Row row)
            {
                return true; // Continue processing
            }
        }
    }
}
```

### Se även

* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


