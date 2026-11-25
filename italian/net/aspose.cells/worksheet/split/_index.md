---
title: "Worksheet.Split"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Divide la finestra"
type: docs
url: /it/net/aspose.cells/worksheet/split/
---
## Worksheet.Split method

Dividi la finestra.

```csharp
public void Split()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodSplitDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio per dimostrare la divisione
            worksheet.Cells["A1"].PutValue("Header");
            for (int i = 1; i <= 50; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Data " + i);
            }
            
            // Dividi il foglio di lavoro (non sono necessari parametri)
            worksheet.Split();
            
            // Salva la cartella di lavoro
            workbook.Save("WorksheetSplitDemo.xml", SaveFormat.SpreadsheetML);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


