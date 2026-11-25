---
title: "Range.Worksheet"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà Range. Ottiene l'oggetto Worksheet che contiene questo intervallo"
type: docs
url: /it/net/aspose.cells/range/worksheet/
---
## Range.Worksheet property

Ottiene l'oggetto `Worksheet` che contiene questo intervallo.

```csharp
public Worksheet Worksheet { get; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangePropertyWorksheetDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Accedi al primo foglio di lavoro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un intervallo denominato
            worksheet.Cells["A1"].PutValue("Test");
            worksheet.Cells["B1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            
            // Definisci un intervallo denominato
            int index = workbook.Worksheets.Names.Add("MyRange");
            Name name = workbook.Worksheets.Names[index];
            name.RefersTo = "=Sheet1!$A$1:$B$2";
            
            // Ottieni l'intervallo per nome (qualifica completamente Range per evitare ambiguità)
            Aspose.Cells.Range range = workbook.Worksheets.GetRangeByName("MyRange");
            
            // Dimostrare l'uso della proprietà Worksheet
            Console.WriteLine("Range belongs to worksheet: " + range.Worksheet.Name);
            
            // Usa la proprietà Worksheet per modificare le celle
            range.Worksheet.Cells["A1"].PutValue("Updated");
            
            // Salva la cartella di lavoro
            workbook.Save("RangePropertyWorksheetDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [Worksheet](../../worksheet/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


