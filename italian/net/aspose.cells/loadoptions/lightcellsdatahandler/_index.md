---
title: "LoadOptions.LightCellsDataHandler"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà LoadOptions. Il gestore dei dati per l'elaborazione dei dati delle celle durante la lettura del file modello"
type: docs
url: /it/net/aspose.cells/loadoptions/lightcellsdatahandler/
---
## LoadOptions.LightCellsDataHandler property

Il gestore dei dati per l'elaborazione dei dati delle celle durante la lettura del file modello.

```csharp
public LightCellsDataHandler LightCellsDataHandler { get; set; }
```

### Esempi

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
            // Crea un LightCellsDataHandler personalizzato per elaborare i dati delle celle
            var dataHandler = new CustomLightCellsDataHandler();
            
            // Crea le opzioni di caricamento e imposta il gestore dei dati
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LightCellsDataHandler = dataHandler;

            // Carica la cartella di lavoro con il gestore personalizzato
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
            // Puoi elaborare i dati delle righe qui, se necessario
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

### Vedi anche

* interface [LightCellsDataHandler](../../lightcellsdatahandler/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


