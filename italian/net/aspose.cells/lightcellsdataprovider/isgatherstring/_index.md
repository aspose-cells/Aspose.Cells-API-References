---
title: "LightCellsDataProvider.IsGatherString"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo LightCellsDataProvider. Verifica se il valore stringa corrente della cella deve essere raccolto in un pool globale"
type: docs
url: /it/net/aspose.cells/lightcellsdataprovider/isgatherstring/
---
## LightCellsDataProvider.IsGatherString method

Verifica se il valore stringa corrente della cella deve essere raccolto in un pool globale.

```csharp
public bool IsGatherString()
```

### Valore di ritorno

true se il valore stringa deve essere raccolto in un pool globale per il file risultante.

### Osservazioni

Raccogliere i valori stringa è vantaggioso solo quando ci sono molte stringhe duplicate per le celle fornite da questa implementazione. In questa situazione la raccolta delle stringhe farà risparmiare molta memoria e genererà un file risultante più piccolo. Se ci sono molte stringhe per le celle fornite da LightCellsDataProvider ma poche sono identiche, la raccolta delle stringhe richiederà più memoria e tempo e non offrirà vantaggi per il file risultante.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderMethodIsGatherStringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Clear();
            
            var saveOptions = new OoxmlSaveOptions
            {
                LightCellsDataProvider = new CustomLightCellsDataProvider()
            };

            try
            {
                workbook.Save("IsGatherStringDemo.xlsx", saveOptions);
                Console.WriteLine("Workbook saved with IsGatherString implementation");
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
            private readonly object[,] data = new object[3, 2]
            {
                { "Product", "Price" },
                { "Laptop", 1200.50 },
                { "Phone", 899.99 }
            };

            public bool StartSheet(int sheetIndex)
            {
                return sheetIndex == 0;
            }

            public int NextRow()
            {
                rowIndex++;
                cellIndex = -1;
                return rowIndex < 3 ? rowIndex : -1;
            }

            public void StartRow(Row row)
            {
                row.Height = 15;
            }

            public int NextCell()
            {
                cellIndex++;
                return cellIndex < 2 ? cellIndex : -1;
            }

            public void StartCell(Cell cell)
            {
                cell.PutValue(data[rowIndex, cellIndex]);
            }

            public bool IsGatherString()
            {
                // Raccogli solo le stringhe per la riga di intestazione (rowIndex 0)
                return rowIndex == 0;
            }
        }
    }
}
```

### Vedi anche

* interface [LightCellsDataProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


