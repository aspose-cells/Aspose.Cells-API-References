---
title: "Range.RefersTo"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Range. Ottiene gli intervalli a cui si riferisce"
type: docs
url: /it/net/aspose.cells/range/refersto/
---
## Range.RefersTo property

Ottiene a cosa si riferisce l'intervallo.

```csharp
public string RefersTo { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyRefersToDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi alcuni dati alle celle
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            
            // Crea un intervallo denominato
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            
            // Imposta la proprietà RefersTo per l'intervallo denominato
            name.RefersTo = "=Sheet1!$A$1:$A$3";
            
            // Ottieni gli intervalli a cui fa riferimento il nome
            Aspose.Cells.Range[] ranges = name.GetRanges();
            
            // Visualizza la proprietà RefersTo del primo intervallo
            Console.WriteLine("Named range refers to: " + ranges[0].RefersTo);
            
            // Crea una formula che utilizza l'intervallo denominato
            worksheet.Cells["B1"].Formula = "=SUM(MyRange)";
            
            // Calcola la formula
            Console.WriteLine("Sum of named range: " + worksheet.Cells["B1"].Value);
        }
    }
}
```

### Vedi anche

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


