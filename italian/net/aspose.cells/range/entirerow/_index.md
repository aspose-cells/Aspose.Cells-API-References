---
title: "Range.EntireRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Range. Restituisce un oggetto Range che rappresenta l'intera riga o le righe che contengono l'intervallo specificato"
type: docs
url: /it/net/aspose.cells/range/entirerow/
---
## Range.EntireRow property

Ottiene un oggetto Range che rappresenta l'intera riga (o le righe) che contiene l'intervallo specificato.

```csharp
public Range EntireRow { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyEntireRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Inserisci alcuni dati di esempio nella prima riga
            for (int col = 0; col < 5; col++)
            {
                sheet.Cells[0, col].PutValue($"Header {col + 1}");
            }

            // Ottieni l'intera prima riga usando la proprietà EntireRow
            Aspose.Cells.Range entireRow = sheet.Cells.CreateRange("A1").EntireRow;

            // Copia la prima riga nella terza riga
            Aspose.Cells.Range destination = sheet.Cells.CreateRange("A3").EntireRow;
            destination.Copy(entireRow);

            // Salva la cartella di lavoro
            workbook.Save("EntireRowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


