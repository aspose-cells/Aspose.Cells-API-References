---
title: "Cell.SharedStyleIndex"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Cell. Restituisce l'indice di stile condiviso delle celle nel pool di stili"
type: docs
url: /it/net/aspose.cells/cell/sharedstyleindex/
---
## Cell.SharedStyleIndex property

Ottiene l'indice di stile condiviso della cella nel pool di stili.

```csharp
public int SharedStyleIndex { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertySharedStyleIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea uno stile e imposta alcune proprietà
            Style style = workbook.CreateStyle();
            style.Font.Name = "Arial";
            style.Font.Size = 12;
            style.Font.IsBold = true;

            // Applica lo stile alla cella A1
            worksheet.Cells["A1"].SetStyle(style);

            // Ottieni l'indice di stile condiviso della cella A1
            int sharedStyleIndex = worksheet.Cells["A1"].SharedStyleIndex;

            // Recupera lo stile dal pool di stili usando l'indice
            Style retrievedStyle = workbook.GetStyleInPool(sharedStyleIndex);

            // Stampa le informazioni sullo stile per verificare
            Console.WriteLine("Font Name: " + retrievedStyle.Font.Name);
            Console.WriteLine("Font Size: " + retrievedStyle.Font.Size);
            Console.WriteLine("Is Bold: " + retrievedStyle.Font.IsBold);
        }
    }
}
```

### Vedi anche

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


