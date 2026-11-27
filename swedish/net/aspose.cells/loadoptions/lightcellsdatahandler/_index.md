---
title: "LoadOptions.LightCellsDataHandler"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions-egenskap. Databehandlaren för att bearbeta celldata när mallfilen läses."
type: docs
url: /sv/net/aspose.cells/loadoptions/lightcellsdatahandler/
---
## LoadOptions.LightCellsDataHandler property

Datahanteraren för bearbetning av celldata när mallfilen läses.

```csharp
public LightCellsDataHandler LightCellsDataHandler { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyLightCellsDataHandlerDemo
    {
        public static void Run()
        {
            // Skapa en anpassad LightCellsDataHandler för att bearbeta celldata
            var dataHandler = new CustomLightCellsDataHandler();
            
            // Skapa inläsningsalternativ och ange databehandlaren
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LightCellsDataHandler = dataHandler;

            // Läs in arbetsboken med den anpassade hanteraren
            using (Workbook workbook = new Workbook("sample.xlsx", loadOptions))
            {
                Console.WriteLine("Workbook processed successfully with LightCellsDataHandler");
            }
        }
    }

    public class CustomLightCellsDataHandler : LightCellsDataHandler
    {
        public bool StartSheet(Worksheet sheet)
        {
            Console.WriteLine($"Processing sheet: {sheet.Name}");
            return true; // Continue processing this sheet
        }

        public bool StartRow(int rowIndex)
        {
            Console.WriteLine($"  Starting row: {rowIndex}");
            return true; // Continue processing this row
        }

        public bool ProcessRow(Row row)
        {
            // Du kan bearbeta raddata här om det behövs
            return true;
        }

        public bool StartCell(int columnIndex)
        {
            Console.WriteLine($"    Starting cell at column: {columnIndex}");
            return true; // Continue processing this cell
        }

        public bool ProcessCell(Cell cell)
        {
            Console.WriteLine($"      Cell[{cell.Row},{cell.Column}]: {cell.Value}");
            return true;
        }
    }
}
```

### Se även

* interface [LightCellsDataHandler](../../lightcellsdatahandler/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


