---
title: "CellRichValue.AltText"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellRichValue-egenskap. Hämtar alt‑texten som är associerad med bilden"
type: docs
url: /sv/net/aspose.cells/cellrichvalue/alttext/
---
## CellRichValue.AltText property

Hämtar alternativ text som är associerad med bilden.

```csharp
public virtual string AltText { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellRichValuePropertyAltTextDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["C4"];
            
            cell.GetRichValue().AltText = "test alt text";
            
            Console.WriteLine("AltText: " + cell.GetRichValue().AltText);
        }
    }
}
```

### Se även

* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


