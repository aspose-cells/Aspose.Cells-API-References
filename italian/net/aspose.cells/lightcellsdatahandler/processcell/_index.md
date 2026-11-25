---
title: "LightCellsDataHandler.ProcessCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo LightCellsDataHandler. Inizia a elaborare una cella"
type: docs
url: /it/net/aspose.cells/lightcellsdatahandler/processcell/
---
## LightCellsDataHandler.ProcessCell method

Inizia a elaborare una cella.

```csharp
public bool ProcessCell(Cell cell)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cella | Cella | Oggetto Cell attualmente in elaborazione |

### Valore di ritorno

indica se questa cella deve essere mantenuta nel modello delle celle del foglio corrente. Di solito dovrebbe essere false in modo che tutte le celle non vengano mantenute in memoria dopo l'elaborazione, risparmiando così memoria. Per alcuni scopi speciali, ad esempio se l'utente deve accedere a determinate celle in seguito, dopo che l'intera cartella di lavoro è stata elaborata, l'utente può far restituire true a questo metodo per mantenere quelle celle speciali nel modello Cells e accedervi successivamente tramite API come Cells[row, column]. Tuttavia, mantenere i dati delle celle nel modello Cells richiede più memoria e, se tutte le celle vengono mantenute, la lettura del file modello in modalità LightCells diventa identica alla lettura in modalità normale.

### Osservazioni

Verrà chiamato dopo che i dati di una cella sono stati letti.

### Esempi

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
                // Crea file dati temporaneo
                File.WriteAllText("input.txt", "A,B,C\n10,20,30\n40,50,60");

                // Crea opzioni di caricamento con gestore light cells personalizzato
                LoadOptions loadOptions = new LoadOptions(LoadFormat.Csv);
                var handler = new CustomLightCellsDataHandler();
                loadOptions.LightCellsDataHandler = handler;

                // Carica la cartella di lavoro con gestore personalizzato
                Workbook workbook = new Workbook("input.txt", loadOptions);

                // Salva i risultati elaborati
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
                // Raddoppia i valori numerici e contrassegna le stringhe
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

### Vedi anche

* class [Cell](../../cell/)
* interface [LightCellsDataHandler](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


