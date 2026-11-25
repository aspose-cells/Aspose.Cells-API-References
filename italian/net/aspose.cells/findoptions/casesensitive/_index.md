---
title: "FindOptions.CaseSensitive"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FindOptions. Indica se la stringa cercata è sensibile al maiuscolo/minuscolo"
type: docs
url: /it/net/aspose.cells/findoptions/casesensitive/
---
## FindOptions.CaseSensitive property

Indica se la stringa cercata è sensibile al maiuscolo/minuscolo.

```csharp
public bool CaseSensitive { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyCaseSensitiveDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta dati di esempio
            worksheet.Cells["A1"].PutValue("ABC");
            worksheet.Cells["A2"].PutValue("abc");
            worksheet.Cells["A3"].PutValue("BcD");

            FindOptions options = new FindOptions();
            options.CaseSensitive = true;
            
            // Cerca "bc" con sensibilità al maiuscolo/minuscolo
            Cell cell = worksheet.Cells.Find("bc", null, options);
            
            Console.WriteLine(cell == null ? "Not found (case sensitive)" : $"Found at: {cell.Name}");
            
            options.CaseSensitive = false;
            cell = worksheet.Cells.Find("bc", null, options);
            
            Console.WriteLine(cell == null ? "Not found" : $"Found at: {cell.Name}");
        }
    }
}
```

### Vedi anche

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


