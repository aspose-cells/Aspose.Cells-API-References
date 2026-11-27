---
title: "MsoLineFormat.IsVisible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoLineFormat‑egenskap. Anger om objektet är synligt"
type: docs
url: /sv/net/aspose.cells.drawing/msolineformat/isvisible/
---
## MsoLineFormat.IsVisible property

Anger om objektet är synligt.

```csharp
public bool IsVisible { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangulär form med synlig kant
            var shape1 = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            shape1.LineFormat.IsVisible = true;

            // Lägg till en oval form med osynlig kant
            var shape2 = worksheet.Shapes.AddOval(2, 0, 150, 100, 100, 100);
            shape2.LineFormat.IsVisible = false;

            // Verifiera och skriv ut värdena för IsVisible‑egenskapen
            Console.WriteLine("Rectangle border visible: " + shape1.LineFormat.IsVisible);
            Console.WriteLine("Oval border visible: " + shape2.LineFormat.IsVisible);

            // Spara arbetsboken
            workbook.Save("MsoLineFormat_IsVisible_Demo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


