---
title: "Worksheet.RemoveAutoFilter"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Worksheet. Rimuove il filtro automatico del foglio di lavoro"
type: docs
url: /it/net/aspose.cells/worksheet/removeautofilter/
---
## Worksheet.RemoveAutoFilter method

Rimuove il filtro automatico del worksheet.

```csharp
public void RemoveAutoFilter()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRemoveAutoFilterDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aggiungi dati di esempio
            worksheet.Cells["A1"].PutValue("Header");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["A3"].PutValue("Data2");
            
            // Applica filtro automatico
            worksheet.AutoFilter.Range = "A1:A3";
            
            Console.WriteLine("AutoFilter applied: " + worksheet.HasAutofilter);
            
            // Rimuovi il filtro automatico
            worksheet.RemoveAutoFilter();
            
            Console.WriteLine("AutoFilter after removal: " + worksheet.HasAutofilter);
        }
    }
}
```

### Vedi anche

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


