---
title: "LightCellsDataProvider.StartCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo LightCellsDataProvider. Inizia a salvare i dati di una cella"
type: docs
url: /it/net/aspose.cells/lightcellsdataprovider/startcell/
---
## LightCellsDataProvider.StartCell method

Inizia a salvare i dati di una cella.

```csharp
public void StartCell(Cell cell)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cell | Cell | Oggetto Cell per l'implementazione che deve riempire i dati. Il suo indice di colonna è il valore restituito dall'ultima chiamata di [`NextCell`](../nextcell/). Se la cella è stata inizializzata nel modello interno delle celle, verrà utilizzato l'oggetto cella esistente. Altrimenti verrà utilizzato un oggetto Cell temporaneo per l'implementazione che deve riempire i dati. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodStartCellWithCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea una cella da usare come parametro
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Data");
            
            // Crea un provider di dati personalizzato
            var saveOptions = new OoxmlSaveOptions
            {
                LightCellsDataProvider = new CustomLightCellsDataProvider()
            };

            try
            {
                workbook.Save("StartCellWithCellDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with StartCell implementation");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class CustomLightCellsDataProvider : LightCellsDataProvider
        {
            private int rowIndex = -1;
            private int cellIndex = -1;
            private readonly int totalRows = 5;
            private readonly int totalCells = 3;

            public bool StartSheet(int sheetIndex)
            {
                return sheetIndex == 0;
            }

            public int NextRow()
            {
                rowIndex++;
                cellIndex = -1;
                return rowIndex < totalRows ? rowIndex : -1;
            }

            public void StartRow(Row row)
            {
                row.Height = 15;
            }

            public int NextCell()
            {
                cellIndex++;
                return cellIndex < totalCells ? cellIndex : -1;
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue($"Row {cell.Row + 1}, Col {cell.Column + 1}");
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

* class [Cell](../../cell/)
* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


