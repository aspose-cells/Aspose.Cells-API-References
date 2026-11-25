---
title: "LightCellsDataProvider.StartSheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo LightCellsDataProvider. Inizia a salvare un foglio di lavoro"
type: docs
url: /it/net/aspose.cells/lightcellsdataprovider/startsheet/
---
## LightCellsDataProvider.StartSheet method

Inizia a salvare un foglio di lavoro.

```csharp
public bool StartSheet(int sheetIndex)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | Int32 | indice del foglio corrente da salvare. |

### Valore di ritorno

true se questo provider fornirà dati per il foglio specificato; false se il foglio specificato deve utilizzare il suo modello dati normale (Cells).

### Osservazioni

Verrà chiamato all'inizio del salvataggio di un foglio di lavoro durante il salvataggio di una cartella di lavoro. Se il provider ha bisogno di fare riferimento a

```csharp
sheetIndex
```

successivamente nel metodo startRow(Row) o startCell(Cell), cioè, se il processo ha bisogno di sapere quale foglio di lavoro è in fase di elaborazione, l'implementazione dovrebbe conservare il

```csharp
sheetIndex
```

valore qui.

### Esempi

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
                
                // Crea un provider di dati personalizzato e salva in modalità light cells
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

            // Chiamato all'inizio dell'elaborazione di un foglio di lavoro
            public bool StartSheet(int sheetIndex)
            {
                Console.WriteLine($"Processing sheet index: {sheetIndex}");
                // Elabora solo il primo foglio (indice 0)
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

### Vedi anche

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


