---
title: "LightCellsDataProvider.NextCell"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo LightCellsDataProvider. Ottiene la prossima cella da salvare"
type: docs
url: /it/net/aspose.cells/lightcellsdataprovider/nextcell/
---
## LightCellsDataProvider.NextCell method

Ottiene la prossima cella da salvare.

```csharp
public int NextCell()
```

### Valore di ritorno

indice di colonna della prossima cella da salvare. -1 indica che è stata raggiunta la fine dei dati della riga corrente e non ci sono altre celle da salvare.

### Osservazioni

Verrà chiamato all'inizio del salvataggio di una cella.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodNextCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Clear();
            
            var provider = new DemoLightCellsDataProvider();
            XlsSaveOptions saveOptions = new XlsSaveOptions { LightCellsDataProvider = provider };

            try
            {
                workbook.Save("NextCellDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with LightCellsDataProvider implementation");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }

        private class DemoLightCellsDataProvider : LightCellsDataProvider
        {
            private int rowIndex = -1;
            private int cellIndex = -1;
            private readonly object[,] data = new object[2, 2]
            {
                { "Column1", "Column2" },
                { 100, 200 }
            };

            public bool StartSheet(int sheetIndex) => sheetIndex == 0;

            public int NextRow()
            {
                rowIndex++;
                cellIndex = -1;
                return rowIndex < 2 ? 1 : 0;
            }

            public void StartRow(Row row) { }

            public int NextCell()
            {
                cellIndex++;
                return cellIndex < 2 ? 1 : 0;
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue(data[rowIndex, cellIndex]);
            }

            public bool IsGatherString() => false;
        }
    }
}
```

### Vedi anche

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


