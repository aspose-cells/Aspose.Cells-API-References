---
title: "FindOptions.CaseSensitive"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FindOptions‑Eigenschaft. Gibt an, ob die gesuchte Zeichenkette Groß‑/Kleinschreibung beachtet"
type: docs
url: /de/net/aspose.cells/findoptions/casesensitive/
---
## FindOptions.CaseSensitive property

Gibt an, ob die gesuchte Zeichenfolge Groß‑ und Kleinschreibung beachtet.

```csharp
public bool CaseSensitive { get; set; }
```

### Beispiele

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
            
            // Beispieldaten festlegen
            worksheet.Cells["A1"].PutValue("ABC");
            worksheet.Cells["A2"].PutValue("abc");
            worksheet.Cells["A3"].PutValue("BcD");

            FindOptions options = new FindOptions();
            options.CaseSensitive = true;
            
            // Suche nach "bc" mit Groß-/Kleinschreibung
            Cell cell = worksheet.Cells.Find("bc", null, options);
            
            Console.WriteLine(cell == null ? "Not found (case sensitive)" : $"Found at: {cell.Name}");
            
            options.CaseSensitive = false;
            cell = worksheet.Cells.Find("bc", null, options);
            
            Console.WriteLine(cell == null ? "Not found" : $"Found at: {cell.Name}");
        }
    }
}
```

### Siehe auch

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


