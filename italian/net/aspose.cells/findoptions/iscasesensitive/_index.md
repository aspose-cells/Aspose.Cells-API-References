---
title: "FindOptions.IsCaseSensitive"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà FindOptions. Indica se la stringa cercata è sensibile al maiuscolo/minuscolo"
type: docs
url: /it/net/aspose.cells/findoptions/iscasesensitive/
---
## FindOptions.IsCaseSensitive property

Indica se la stringa cercata è sensibile al maiuscolo/minuscolo.

```csharp
[Obsolete("Use FindOptions.CaseSensitive property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsCaseSensitive { get; set; }
```

### Osservazioni

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà FindOptions.CaseSensitive. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2010. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyIsCaseSensitiveDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Imposta dati di esempio
            worksheet.Cells["A1"].PutValue("ABC");
            worksheet.Cells["A2"].PutValue("abc");
            worksheet.Cells["A3"].PutValue("AbC");

            FindOptions options = new FindOptions();
            options.IsCaseSensitive = true;
            
            // Trova corrispondenza sensibile al maiuscolo/minuscolo
            Cell cell = worksheet.Cells.Find("abc", null, options);
            
            Console.WriteLine("Case-sensitive search for 'abc' found at: " + 
                              (cell != null ? cell.Name : "No match"));
        }
    }
}
```

### Vedi anche

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


