---
title: "Cell.GetRichValue"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Cell. Ottiene il valore ricco della cella"
type: docs
url: /it/net/aspose.cells/cell/getrichvalue/
---
## Cell.GetRichValue method

Ottiene il valore ricco della cella.

```csharp
public CellRichValue GetRichValue()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetRichValueDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook wb = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet ws = wb.Worksheets[0];
            
            // Imposta un valore di testo ricco nella cella A1
            ws.Cells["A1"].PutValue("This is rich text");
            
            // Ottieni il valore ricco dalla cella A1
            CellRichValue richValue = ws.Cells["A1"].GetRichValue();
            
            // Visualizza il valore di testo ricco
            Console.WriteLine("Rich Text Value: " + ws.Cells["A1"].StringValue);
            
            // Salva la cartella di lavoro
            wb.Save("RichValueDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [CellRichValue](../../cellrichvalue/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


