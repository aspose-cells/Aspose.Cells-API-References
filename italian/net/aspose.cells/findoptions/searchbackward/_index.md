---
title: "FindOptions.SearchBackward"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FindOptions. Indica se cercare all'indietro le celle"
type: docs
url: /it/net/aspose.cells/findoptions/searchbackward/
---
## FindOptions.SearchBackward property

Indica se cercare all'indietro le celle.

```csharp
public bool SearchBackward { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertySearchBackwardDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Configura dati di esempio
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["B2"].PutValue("abc");
            worksheet.Cells["C3"].PutValue("abc");

            FindOptions options = new FindOptions();
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;
            
            // Cerca in avanti (comportamento predefinito)
            options.SearchBackward = false;
            Cell foundForward = worksheet.Cells.Find("abc", null, options);
            Console.WriteLine($"Forward search found at: {foundForward.Name}");

            // Cerca all'indietro
            options.SearchBackward = true;
            Cell foundBackward = worksheet.Cells.Find("abc", null, options);
            Console.WriteLine($"Backward search found at: {foundBackward.Name}");
        }
    }
}
```

### Vedi anche

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


