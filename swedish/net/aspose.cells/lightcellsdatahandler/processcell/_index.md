---
title: "LightCellsDataHandler.ProcessCell"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LightCellsDataHandler-metoden. Påbörjar bearbetning av en cell"
type: docs
url: /sv/net/aspose.cells/lightcellsdatahandler/processcell/
---
## LightCellsDataHandler.ProcessCell method

Påbörjar bearbetning av en cell.

```csharp
public bool ProcessCell(Cell cell)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cell | Cell | Cellobjekt som för närvarande bearbetas |

### Returvärde

om den här cellen behöver behållas i cellmodellen för det aktuella bladet. Vanligtvis bör den vara false så att alla celler inte behålls i minnet efter att de har bearbetats och minnet därmed sparas. För vissa speciella ändamål, såsom när användaren behöver komma åt vissa celler senare efter att hela arbetsboken har bearbetats, kan användaren låta denna metod returnera true för att behålla de speciella cellerna i Cells-modellen och komma åt dem senare via API:er som Cells[row, column]. Dock kräver det att hålla celldata i Cells-modellen mer minne, och om alla celler behålls blir läsning av mallfilen i LightCells-läge samma som att läsa den på normalt sätt.

### Anmärkningar

Den kommer att anropas efter att en cells data har lästs.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class LightCellsDataHandlerMethodProcessCellWithCellDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa temporär datafil
                File.WriteAllText("input.txt", "A,B,C\n10,20,30\n40,50,60");

                // Skapa laddningsalternativ med anpassad LightCells-hanterare
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                var handler = new CustomLightCellsDataHandler();
                loadOptions.LightCellsDataHandler = handler;

                // Läs in arbetsbok med anpassad hanterare
                Workbook workbook = new Workbook("input.txt", loadOptions);

                // Spara bearbetade resultat
                workbook.Save("output.xlsx");
                Console.WriteLine("ProcessCell executed successfully. Check output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ProcessCell: {ex.Message}");
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
                return true; // Process all cells
            }

            public bool ProcessCell(Cell cell)
            {
                // Dubbla numeriska värden och markera strängar
                if (cell.IsNumericValue)
                {
                    cell.PutValue(cell.DoubleValue * 2);
                }
                else if (cell.Type == CellValueType.IsString)
                {
                    cell.PutValue($"TEXT: {cell.StringValue}");
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

* class [Cell](../../cell/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


