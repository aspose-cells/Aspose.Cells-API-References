---
title: "NoneBulletValue.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad NoneBulletValue. Obtiene el tipo del valor de la viñeta"
type: docs
url: /es/net/aspose.cells.drawing.texts/nonebulletvalue/type/
---
## NoneBulletValue.Type property

Obtiene el tipo del valor de la viñeta.

```csharp
public override BulletType Type { get; }
```

### Ejemplos

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

### Ver también

* enum [BulletType](../../bullettype/)
* class [NoneBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


