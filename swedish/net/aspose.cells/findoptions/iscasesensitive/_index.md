---
title: "FindOptions.IsCaseSensitive"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FindOptions-egenskapen. Anger om den sökta strängen är skiftlägeskänslig"
type: docs
url: /sv/net/aspose.cells/findoptions/iscasesensitive/
---
## FindOptions.IsCaseSensitive property

Indikerar om den sökta strängen är skiftlägeskänslig.

```csharp
[Obsolete("Use FindOptions.CaseSensitive property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsCaseSensitive { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället FindOptions.CaseSensitive-egenskapen. Denna egenskap kommer att tas bort 12 månader senare sedan juni 2010. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

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
            
            // Ange exempeldata
            worksheet.Cells["A1"].PutValue("ABC");
            worksheet.Cells["A2"].PutValue("abc");
            worksheet.Cells["A3"].PutValue("AbC");

            FindOptions options = new FindOptions();
            options.IsCaseSensitive = true;
            
            // Sök skiftlägeskänslig matchning
            Cell cell = worksheet.Cells.Find("abc", null, options);
            
            Console.WriteLine("Case-sensitive search for 'abc' found at: " + 
                              (cell != null ? cell.Name : "No match"));
        }
    }
}
```

### Se även

* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


