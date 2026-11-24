---
title: "FindOptions.LookAtType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "FindOptions‑Eigenschaft. Typ ansehen"
type: docs
url: /de/net/aspose.cells/findoptions/lookattype/
---
## FindOptions.LookAtType property

Typ ansehen.

```csharp
public LookAtType LookAtType { get; set; }
```

### Hinweise

Wenn [`RegexKey`](../regexkey/) true ist und der Benutzer die genaue Regel für den Regex angegeben hat, sollte diese Eigenschaft aus Performance‑Gründen auf EntireContent gesetzt werden. Andernfalls werden wir den Suchschlüssel umstrukturieren, um sicherzustellen, dass er gemäß dem jeweiligen Typ übereinstimmen kann. Zum Beispiel, wenn der Typ Contains ist (dies ist der Standardwert für diese Eigenschaft), fügen wir automatisch Wildcards am Anfang und Ende des Suchschlüssels hinzu. In diesem Fall werden die regulären Ausdrücke komplexer und die Leistung wird ebenfalls sinken.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class FindOptionsPropertyLookAtTypeDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe und fügen Sie einige Daten hinzu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Hello World");
            worksheet.Cells["A2"].PutValue("=1+2"); // Formula
            worksheet.Cells["A3"].PutValue("Partial match test");
            worksheet.Cells["A4"].PutValue("=A1&A3"); // Formula concatenating cells

            // Erstelle FindOptions mit LookAtType.EntireContent
            FindOptions options = new FindOptions
            {
                LookInType = LookInType.OnlyFormulas,
                LookAtType = LookAtType.EntireContent
            };

            // Suche nach einer Formel, die exakt "=A1&A3" entspricht
            Cell cell = worksheet.Cells.Find("=A1&A3", null, options);
            Console.WriteLine("Found cell with exact formula match: " + (cell != null ? cell.Name : "null"));

            // Ändern zu teilweiser Übereinstimmung
            options.LookAtType = LookAtType.Contains;
            cell = worksheet.Cells.Find("A3", null, options);
            Console.WriteLine("Found cell containing 'A3' in formula: " + (cell != null ? cell.Name : "null"));
        }
    }
}
```

### Siehe auch

* enum [LookAtType](../../lookattype/)
* class [FindOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


