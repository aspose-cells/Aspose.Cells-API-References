---
title: "NoneBulletValue.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "NoneBulletValue-egenskapen. Hämtar typen av bulletvärdet"
type: docs
url: /sv/net/aspose.cells.drawing.texts/nonebulletvalue/type/
---
## NoneBulletValue.Type property

Hämtar typen av punktlistans värde.

```csharp
public override BulletType Type { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.Texts;

namespace AsposeCellsExamples
{
    public class NoneBulletValuePropertyTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            NoneBulletValue noneBulletValue = new NoneBulletValue();
            BulletType bulletType = noneBulletValue.Type;
            
            Console.WriteLine("Bullet Type: " + bulletType); // Output: None

            workbook.Save("NoneBulletValueExample.xlsx");
        }
    }
}
```

### Se även

* enum [BulletType](../../bullettype/)
* class [NoneBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


