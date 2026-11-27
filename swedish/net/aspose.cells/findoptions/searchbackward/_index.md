---
title: "FindOptions.SearchBackward"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FindOptions-egenskap. Anger om sökningen ska gå bakåt för celler"
type: docs
url: /sv/net/aspose.cells/findoptions/searchbackward/
---
## FindOptions.SearchBackward property

Om sökningen ska gå bakåt för celler.

```csharp
public bool SearchBackward { get; set; }
```

### Exempel

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
            
            // Ställ in exempeldata
            worksheet.Cells["A1"].PutValue("abc");
            worksheet.Cells["B2"].PutValue("abc");
            worksheet.Cells["C3"].PutValue("abc");

            FindOptions options = new FindOptions();
            options.LookInType = LookInType.Values;
            options.LookAtType = LookAtType.Contains;
            
            // Sök framåt (standardbeteende)
            options.SearchBackward = false;
            Cell foundForward = worksheet.Cells.Find("abc", null, options);
            Console.WriteLine($"Forward search found at: {foundForward.Name}");

            // Sök bakåt
            options.SearchBackward = true;
            Cell foundBackward = worksheet.Cells.Find("abc", null, options);
            Console.WriteLine($"Backward search found at: {foundBackward.Name}");
        }
    }
}
```

### Se även

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


