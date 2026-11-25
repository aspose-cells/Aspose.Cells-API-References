---
title: "LightCellsDataProvider.StartRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo LightCellsDataProvider. Inizia a salvare i dati di una riga"
type: docs
url: /it/net/aspose.cells/lightcellsdataprovider/startrow/
---
## LightCellsDataProvider.StartRow method

Inizia a salvare i dati di una riga.

```csharp
public void StartRow(Row row)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| row | Row | Oggetto Row per l'implementazione che deve riempire i dati. Il suo indice di riga è il valore restituito dall'ultima chiamata di [`NextRow`](../nextrow/). Se la riga è stata inizializzata nel modello interno delle celle, verrà utilizzato l'oggetto row esistente. Altrimenti verrà utilizzato un oggetto Row temporaneo per l'implementazione che deve riempire i dati. |

### Osservazioni

Verrà chiamato all'inizio del salvataggio di una riga e dei dati delle sue celle. Se la riga corrente ha alcune proprietà personalizzate come altezza, stile, ...ecc., l'implementazione dovrebbe impostare tali proprietà sull'oggetto Row fornito qui.

### Esempi

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
            
            // Crea un provider di dati personalizzato
            var saveOptions = new OoxmlSaveOptions
            {
                LightCellsDataProvider = new CustomLightCellsDataProvider()
            };

            try
            {
                // Elabora la cartella di lavoro con il nostro provider di dati personalizzato
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
                // Dimostra il metodo StartRow con il parametro Row
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

### Vedi anche

* class [Row](../../row/)
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


