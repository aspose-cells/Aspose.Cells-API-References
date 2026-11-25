---
title: "Worksheet.FirstVisibleRow"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Rappresenta l'indice della prima riga visibile"
type: docs
url: /it/net/aspose.cells/worksheet/firstvisiblerow/
---
## Worksheet.FirstVisibleRow property

Rappresenta l'indice della prima riga visibile.

```csharp
public int FirstVisibleRow { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyFirstVisibleRowDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta alcuni dati di esempio
            for (int i = 0; i < 50; i++)
            {
                worksheet.Cells[i, 0].Value = "Row " + (i + 1);
            }
            
            // Imposta la prima riga visibile alla riga 20
            worksheet.FirstVisibleRow = 20;
            
            // Visualizza la prima riga visibile
            Console.WriteLine("First visible row: " + worksheet.FirstVisibleRow);
            
            // Salva la cartella di lavoro
            workbook.Save("FirstVisibleRowDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


