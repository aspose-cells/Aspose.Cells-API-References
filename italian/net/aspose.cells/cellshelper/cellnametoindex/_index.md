---
title: "CellsHelper.CellNameToIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo di CellsHelper. Ottiene gli indici di riga e colonna della cella secondo il suo nome"
type: docs
url: /it/net/aspose.cells/cellshelper/cellnametoindex/
---
## CellsHelper.CellNameToIndex method

Ottiene gli indici di riga e colonna della cella in base al suo nome.

```csharp
public static void CellNameToIndex(string cellName, out int row, out int column)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | String | Nome della cella. |
| riga | Int32& | Indice di riga di output |
| colonna | Int32& | Indice di colonna di output |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class CellsHelperMethodCellNameToIndexWithStringInt32Int32Demo
    {
        public static void Run()
        {
            // Inizializza le variabili per contenere gli indici di riga e colonna
            int rowIndex = -1;
            int columnIndex = -1;
            string cellName = "C5";

            try
            {
                // Chiama il metodo CellNameToIndex per convertire il nome della cella in indici di riga e colonna
                CellsHelper.CellNameToIndex(cellName, out rowIndex, out columnIndex);

                // Visualizza i risultati
                Console.WriteLine($"Cell name: {cellName}");
                Console.WriteLine($"Row index: {rowIndex}");
                Console.WriteLine($"Column index: {columnIndex}");

                // Crea una cartella di lavoro e dimostra l'uso degli indici
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Accedi alla cella usando gli indici ottenuti
                Cell cell = worksheet.Cells[rowIndex, columnIndex];
                cell.PutValue("Test Value");

                // Salva la cartella di lavoro
                workbook.Save("CellNameToIndexDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing CellNameToIndex method: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* class [CellsHelper](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


