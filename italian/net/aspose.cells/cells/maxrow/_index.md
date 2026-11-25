---
title: "Cells.MaxRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Indice massimo della riga della cella che contiene dati o stile"
type: docs
url: /it/net/aspose.cells/cells/maxrow/
---
## Cells.MaxRow property

Indice di riga massimo della cella che contiene dati o stile.

```csharp
public int MaxRow { get; }
```

### Osservazioni

Restituisce -1 se non esiste alcuna cella che contiene dati o stile nel foglio di lavoro. Questa proprietà deve iterare e controllare dinamicamente celle e righe, quindi è un'operazione che richiede tempo e non dovrebbe essere invocata ripetutamente, ad esempio usandola direttamente come condizione in un ciclo.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Aggiungi alcuni dati di esempio
            cells[0, 0].PutValue("Name");
            cells[0, 1].PutValue("Age");
            cells[1, 0].PutValue("John");
            cells[1, 1].PutValue(30);
            cells[2, 0].PutValue("Alice");
            cells[2, 1].PutValue(25);

            // Ottieni l'indice massimo della riga (basato su zero)
            int maxRow = cells.MaxRow;
            Console.WriteLine("MaxRow before adding new data: " + maxRow);

            // Aggiungi nuovi dati nella riga successiva al massimo indice di riga
            int newRow = maxRow + 1;
            cells[newRow, 0].PutValue("Bob");
            cells[newRow, 1].PutValue(28);

            // Verifica il nuovo massimo indice di riga
            Console.WriteLine("MaxRow after adding new data: " + cells.MaxRow);

            // Salva la cartella di lavoro
            workbook.Save("MaxRowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


