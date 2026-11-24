---
title: "Style.QuotePrefix"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Style-Eigenschaft. Gibt an, ob der Zellenwert mit einem einfachen Anführungszeichen beginnt"
type: docs
url: /de/net/aspose.cells/style/quoteprefix/
---
## Style.QuotePrefix property

Gibt an, ob der Zellenwert mit einem einfachen Anführungszeichen beginnt.

```csharp
public bool QuotePrefix { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class StylePropertyQuotePrefixDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Greifen Sie auf die Zelle B10 zu und setzen Sie ihren Wert
            Cell cell = worksheet.Cells["B10"];
            cell.PutValue("'12345"); // Note the single quote prefix

            // Holen Sie den Stil der Zelle und aktivieren Sie QuotePrefix
            Style style = cell.GetStyle();
            style.QuotePrefix = true;
            cell.SetStyle(style);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");

            // Überprüfen Sie die QuotePrefix-Eigenschaft
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Cell loadedCell = loadedWorkbook.Worksheets[0].Cells["B10"];
            Console.WriteLine("QuotePrefix is set: " + loadedCell.GetStyle().QuotePrefix);
        }
    }
}
```

### Siehe auch

* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


