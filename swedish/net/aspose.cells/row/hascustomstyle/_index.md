---
title: "Row.HasCustomStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Row-egenskap. Anger om denna rad har anpassade stilinställningar som skiljer sig från standardinställningen som ärvs från arbetsboken"
type: docs
url: /sv/net/aspose.cells/row/hascustomstyle/
---
## Row.HasCustomStyle property

Anger om den här raden har anpassade stilinställningar(skiljer sig från standardinställningen som ärvs från arbetsboken).

```csharp
public bool HasCustomStyle { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class RowPropertyHasCustomStyleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Skapa och anpassa en stil
            Style customStyle = workbook.CreateStyle();
            customStyle.BackgroundColor = Color.LightBlue;
            customStyle.Pattern = BackgroundType.Solid;
            
            // Få åtkomst till första raden
            Row row = worksheet.Cells.Rows[0];
            
            // Tillämpa anpassad stil på raden
            row.ApplyStyle(customStyle, new StyleFlag { All = true });
            
            // Kontrollera om raden har anpassad stil (ska vara true)
            bool hasCustomStyle = row.HasCustomStyle;
            Console.WriteLine("Row has custom style: " + hasCustomStyle);
            
            // Spara arbetsboken
            workbook.Save("RowHasCustomStyleDemo.xlsx");
        }
    }
}
```

### Se även

* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


