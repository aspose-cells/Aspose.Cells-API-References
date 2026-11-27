---
title: "SheetSet.Visible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SheetSet-egenskap. Hämtar en uppsättning med synliga blad i arbetsboken i deras ursprungliga ordning"
type: docs
url: /sv/net/aspose.cells.rendering/sheetset/visible/
---
## SheetSet.Visible property

Hämtar en uppsättning med synliga blad i arbetsboken i deras ursprungliga ordning.

```csharp
public static SheetSet Visible { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetSetPropertyVisibleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok med två kalkylblad
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // Dölj det andra kalkylbladet
            workbook.Worksheets[1].IsVisible = false;

            // Ställ in sparalternativ för att bara exportera synliga blad
            PptxSaveOptions saveOptions = new PptxSaveOptions
            {
                SheetSet = SheetSet.Visible
            };

            // Spara arbetsboken (endast synligt blad kommer att exporteras)
            workbook.Save("VisibleSheetsOnly.pptx", saveOptions);

            Console.WriteLine("Workbook saved with only visible sheets exported.");
        }
    }
}
```

### Se även

* class [SheetSet](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


