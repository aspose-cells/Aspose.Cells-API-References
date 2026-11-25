---
title: "Range.RowHeight"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Range. Imposta o restituisce l'altezza delle righe in questo intervallo"
type: docs
url: /it/net/aspose.cells/range/rowheight/
---
## Range.RowHeight property

Imposta o ottiene l'altezza delle righe in questo intervallo

```csharp
public double RowHeight { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRowHeightDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Imposta alcuni dati nella prima riga
            worksheet.Cells["A1"].PutValue("This is a test");
            worksheet.Cells["B1"].PutValue("to demonstrate");
            worksheet.Cells["C1"].PutValue("RowHeight property");

            // Ottieni l'altezza iniziale della riga
            double initialHeight = worksheet.Cells.CreateRange("1:1").RowHeight;
            Console.WriteLine("Initial row height: " + initialHeight);

            // Adatta automaticamente la riga
            worksheet.AutoFitRow(0);

            // Ottieni la nuova altezza della riga dopo l'adattamento automatico
            double newHeight = worksheet.Cells.CreateRange("1:1").RowHeight;
            Console.WriteLine("Row height after auto-fit: " + newHeight);

            // Imposta manualmente una nuova altezza della riga
            worksheet.Cells.CreateRange("1:1").RowHeight = 30;
            Console.WriteLine("Row height after manual set: " + worksheet.Cells.CreateRange("1:1").RowHeight);
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


