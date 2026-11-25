---
title: "Cells.MinDataRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cells. Indice di riga minimo della cella che contiene dati"
type: docs
url: /it/net/aspose.cells/cells/mindatarow/
---
## Cells.MinDataRow property

Indice di riga minimo della cella che contiene dati.

```csharp
public int MinDataRow { get; }
```

### Osservazioni

Restituisce -1 se non esiste alcuna cella che contiene dati. Questa proprietà deve iterare e controllare celle e righe dinamicamente, quindi è un processo dispendioso in termini di tempo e non dovrebbe essere invocata ripetutamente, ad esempio usandola direttamente come condizione in un ciclo.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinDataRowDemo
    {
        public static void Run()
        {
            // Crea una cartella di lavoro
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Popola alcuni dati
            sheet.Cells[0, 0].Value = "Header1";
            sheet.Cells[0, 1].Value = "Header2";
            sheet.Cells[1, 0].Value = "Data1";
            sheet.Cells[1, 1].Value = "Data2";
            sheet.Cells[2, 0].Value = "Data3";
            sheet.Cells[2, 1].Value = "Data4";

            // Dimostra l'uso di MinDataRow
            Console.WriteLine("Minimum data row index: " + sheet.Cells.MinDataRow);
            Console.WriteLine("Maximum data row index: " + sheet.Cells.MaxDataRow);

            // Salva la cartella di lavoro
            workbook.Save("MinDataRowExample.xlsx");
        }
    }
}
```

### Vedi anche

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


