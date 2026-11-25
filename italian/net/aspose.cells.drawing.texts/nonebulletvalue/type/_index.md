---
title: "NoneBulletValue.Type"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà NoneBulletValue. Ottiene il tipo del valore dei punti elenco"
type: docs
url: /it/net/aspose.cells.drawing.texts/nonebulletvalue/type/
---
## NoneBulletValue.Type property

Ottiene il tipo del valore del punto elenco.

```csharp
public override BulletType Type { get; }
```

### Esempi

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

### Vedi anche

* enum [BulletType](../../bullettype/)
* class [NoneBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


