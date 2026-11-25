---
title: "LightCellsDataProvider.NextRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo LightCellsDataProvider. Ottiene la prossima riga da salvare"
type: docs
url: /it/net/aspose.cells/lightcellsdataprovider/nextrow/
---
## LightCellsDataProvider.NextRow method

Ottiene la prossima riga da salvare.

```csharp
public int NextRow()
```

### Valore di ritorno

l'indice della prossima riga da salvare. -1 indica che è stata raggiunta la fine dei dati del foglio corrente e non ci sono altre righe da salvare.

### Osservazioni

Verrà chiamato all'inizio del salvataggio di una riga e dei suoi dati di celle (prima di [`StartRow`](../startrow/)).

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodNextRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Clear();
            workbook.Worksheets.Add("Sheet1");

            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();
            saveOptions.LightCellsDataProvider = new CustomLightCellsDataProvider();

            try
            {
                workbook.Save("LightCellsDataProviderMethodNextRowDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with LightCellsDataProvider implementation.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        private int currentRow = -1;
        private int currentCell = -1;
        private readonly int totalRows = 3;

        public bool StartSheet(int sheetIndex)
        {
            return sheetIndex == 0;
        }

        public int NextRow()
        {
            currentRow++;
            currentCell = -1;
            return currentRow < totalRows ? currentRow : -1;
        }

        public void StartRow(Row row)
        {
            row.Height = 20;
        }

        public int NextCell()
        {
            currentCell++;
            return currentCell < 2 ? currentCell : -1;
        }

        public void StartCell(Cell cell)
        {
            cell.PutValue($"R{currentRow}C{currentCell}");
        }

        public bool IsGatherString()
        {
            return false;
        }
    }
}
```

### Vedi anche

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


