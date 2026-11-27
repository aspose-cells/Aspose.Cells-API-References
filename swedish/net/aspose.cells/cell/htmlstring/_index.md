---
title: "Cell.HtmlString"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Cell‑egenskap. Hämtar och anger HTML‑strängen som innehåller data och vissa format i den här cellen"
type: docs
url: /sv/net/aspose.cells/cell/htmlstring/
---
## Cell.HtmlString property

Hämtar och anger html-strängen som innehåller data och vissa format i den här cellen.

```csharp
public string HtmlString { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellPropertyHtmlStringDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbokinstans
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till cells-samlingen
            Cells cells = worksheet.Cells;
            
            // Ange HTML‑sträng med formatering till cell A1
            cells["A1"].HtmlString = "This is <b>bold</b> and <i>italic</i> text<br>with a line break";
            
            // Spara arbetsboken
            workbook.Save("HtmlStringDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


