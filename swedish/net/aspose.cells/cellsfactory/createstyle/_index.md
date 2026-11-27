---
title: "CellsFactory.CreateStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "CellsFactory‑metod. Skapar en ny stil"
type: docs
url: /sv/net/aspose.cells/cellsfactory/createstyle/
---
## CellsFactory.CreateStyle method

Skapar en ny stil.

```csharp
public Style CreateStyle()
```

### Returvärde

Returnerar ett stilobjekt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class CellsFactoryMethodCreateStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Skapa en stil med CellsFactory
            Style style = new CellsFactory().CreateStyle();
            
            // Ställ in kant‑egenskaper för stilen
            style.SetBorder(BorderType.BottomBorder, CellBorderType.Thick, Color.Black);
            
            // Tillämpa stilen på en cell
            workbook.Worksheets[0].Cells["A1"].Value = "Hello World";
            workbook.Worksheets[0].Cells["A1"].SetStyle(style);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [Style](../../style/)
* class [CellsFactory](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


