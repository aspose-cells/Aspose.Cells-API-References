---
title: "LoadOptions.LightCellsDataHandler"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadOptions-Eigenschaft. Der Datenhandler zur Verarbeitung von Zellendaten beim Lesen der Vorlagendatei"
type: docs
url: /de/net/aspose.cells/loadoptions/lightcellsdatahandler/
---
## LoadOptions.LightCellsDataHandler property

Der Datenhandler zur Verarbeitung von Zellen­daten beim Lesen der Vorlagendatei.

```csharp
public LightCellsDataHandler LightCellsDataHandler { get; set; }
```

### Beispiele

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
            // Einen benutzerdefinierten LightCellsDataHandler erstellen, um Zellendaten zu verarbeiten
            var dataHandler = new CustomLightCellsDataHandler();
            
            // Ladeoptionen erstellen und den Datenhandler setzen
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LightCellsDataHandler = dataHandler;

            // Arbeitsmappe mit dem benutzerdefinierten Handler laden
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
            // Sie können hier Zeilendaten verarbeiten, falls nötig
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

### Siehe auch

* interface [LightCellsDataHandler](../../lightcellsdatahandler/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


