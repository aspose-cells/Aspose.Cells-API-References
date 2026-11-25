---
title: "Row.Height"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Row proprietà. Ottiene e imposta l'altezza della riga in unità di punti"
type: docs
url: /it/net/aspose.cells/row/height/
---
## Row.Height property

Ottiene e imposta l'altezza della riga in unità di punti.

```csharp
public double Height { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RowPropertyHeightDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta l'altezza della riga per la prima riga
            Row row = worksheet.Cells.Rows[0];
            row.Height = 30;
            
            // Aggiungi alcuni dati alla riga
            worksheet.Cells["A1"].PutValue("Row with custom height");
            
            // Verifica e visualizza l'altezza della riga
            Console.WriteLine("Row 1 Height: " + row.Height);
            
            // Salva la cartella di lavoro
            workbook.Save("RowHeightDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


