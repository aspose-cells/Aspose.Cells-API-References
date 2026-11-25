---
title: "LightCellsDataHandler.StartCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo LightCellsDataHandler. Prepara l'elaborazione di una cella"
type: docs
url: /it/net/aspose.cells/lightcellsdatahandler/startcell/
---
## LightCellsDataHandler.StartCell method

Prepara l'elaborazione di una cella.

```csharp
public bool StartCell(int columnIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | Int32 | indice di colonna della cella da elaborare |

### Valore di ritorno

indica se questa cella deve essere elaborata. false per ignorare la cella e controllare la successiva fino a raggiungere la fine dei dati delle celle della riga corrente.

### Osservazioni

Verrà chiamato quando si raggiunge una cella esistente nella riga corrente. La riga corrente è la riga dell'ultima chiamata di [`ProcessRow`](../processrow/).

### Esempi

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
                // Crea un file di input temporaneo
                File.WriteAllText("input.csv", "Column1,Column2,Column3\n1,2,3\n4,5,6");

                // Crea opzioni di caricamento con gestore light cells personalizzato
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                var handler = new CustomLightCellsDataHandler();
                loadOptions.LightCellsDataHandler = handler;

                // Carica la cartella di lavoro con gestore personalizzato
                Workbook workbook = new Workbook("input.csv", loadOptions);

                // Salva la cartella di lavoro elaborata
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
                // Elabora solo le celle nella colonna indice 1 (seconda colonna)
                return columnIndex == 1;
            }

            public bool ProcessCell(Cell cell)
            {
                // Raddoppia il valore delle celle nella seconda colonna
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

### Vedi anche

* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


