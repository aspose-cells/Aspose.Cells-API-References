---
title: "Classe CellRichValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.CellRichValue classe. Rappresenta il valore ricco della cella"
type: docs
url: /it/net/aspose.cells/cellrichvalue/
---
## CellRichValue class

Rappresenta il valore ricco della cella.

```csharp
public abstract class CellRichValue
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| virtual [AltText](../../aspose.cells/cellrichvalue/alttext/) { get; set; } | Ottiene il testo alternativo associato all'immagine. |
| virtual [ErrorValue](../../aspose.cells/cellrichvalue/errorvalue/) { get; } | Ottiene il tipo di valore di errore della cella. |
| virtual [Image](../../aspose.cells/cellrichvalue/image/) { get; } | Ottiene i dati dell'immagine della cella. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassCellRichValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta un valore ricco nella cella A1
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Rich Value");
            
            // Ottieni il valore ricco dalla cella A1
            CellRichValue richValue = cell.GetRichValue();
            
            // Visualizza le proprietà del valore ricco
            Console.WriteLine("Rich Value: " + richValue.ToString());
            
            // Salva la cartella di lavoro
            workbook.Save("RichValueDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


