---
title: "Worksheet.HasAutofilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Worksheet. Indica se questo foglio di lavoro ha il filtro automatico"
type: docs
url: /it/net/aspose.cells/worksheet/hasautofilter/
---
## Worksheet.HasAutofilter property

Indica se questo foglio di lavoro ha un filtro automatico.

```csharp
public bool HasAutofilter { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyHasAutofilterDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);
            
            // Imposta il filtro automatico
            worksheet.AutoFilter.Range = "A1:B3";
            
            // Verifica se il foglio di lavoro ha il filtro automatico
            Console.WriteLine("Worksheet has autofilter: " + worksheet.HasAutofilter);
            
            // Salva la cartella di lavoro
            workbook.Save("output.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


