---
title: "DeleteBlankOptions.EmptyStringAsBlank"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DeleteBlankOptions egenskap. Anger om en cell ska betraktas som tom när dess värde är en tom sträng. Standardvärdet är true"
type: docs
url: /sv/net/aspose.cells/deleteblankoptions/emptystringasblank/
---
## DeleteBlankOptions.EmptyStringAsBlank property

Anger om en cell ska betraktas som tom när dess värde är en tom sträng. Standardvärdet är true.

```csharp
public bool EmptyStringAsBlank { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEmptyStringAsBlankDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll kalkylbladet med data inklusive tomma strängar
            worksheet.Cells["A1"].PutValue("Data");
            worksheet.Cells["A2"].PutValue("");
            worksheet.Cells["A3"].PutValue("More Data");
            worksheet.Cells["A4"].PutValue("");
            worksheet.Cells["A5"].PutValue("Even More Data");

            // Konfigurera DeleteBlankOptions med EmptyStringAsBlank satt till true
            DeleteBlankOptions options = new DeleteBlankOptions
            {
                EmptyStringAsBlank = true
            };

            // Ta bort rader som innehåller tomma strängar (behandlas som tomma)
            worksheet.Cells.DeleteBlankRows(options);

            // Spara resultatet
            workbook.Save("DeleteBlankOptions_EmptyStringAsBlank_Output.xlsx");
        }
    }
}
```

### Se även

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


