---
title: "Cells.MinRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Indice di riga minimo della cella che contiene dati o stile"
type: docs
url: /it/net/aspose.cells/cells/minrow/
---
## Cells.MinRow property

Indice di riga minimo della cella che contiene dati o stile.

```csharp
public int MinRow { get; }
```

### Osservazioni

Questa proprietà deve iterare e controllare celle e righe in modo dinamico, quindi è un processo che richiede tempo e non dovrebbe essere invocata ripetutamente, ad esempio usandola direttamente come condizione in un ciclo.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi alcuni dati per dimostrare MinRow
            cells["A1"].PutValue("Data in first row");
            cells["B5"].PutValue("Data in fifth row");

            // Visualizza le informazioni di MinRow
            Console.WriteLine("Minimum used row: " + cells.MinRow);
            Console.WriteLine("Maximum used row: " + cells.MaxRow);

            // Cancella i contenuti a partire da MinRow
            cells.ClearContents(cells.MinRow, cells.MinColumn, cells.MaxRow, cells.MaxColumn);

            // Verifica la cancellazione controllando se le celle sono vuote
            Console.WriteLine("A1 after clearing: " + (cells["A1"].Value == null ? "Empty" : "Not empty"));
            Console.WriteLine("B5 after clearing: " + (cells["B5"].Value == null ? "Empty" : "Not empty"));
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


