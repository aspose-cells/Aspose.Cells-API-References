---
title: "NoneBulletValue.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية NoneBulletValue. تحصل على نوع قيمة الرصاصات"
type: docs
url: /ar/net/aspose.cells.drawing.texts/nonebulletvalue/type/
---
## NoneBulletValue.Type property

يحصل على نوع قيمة النقطة.

```csharp
public override BulletType Type { get; }
```

### أمثلة

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

### انظر أيضًا

* enum [BulletType](../../bullettype/)
* class [NoneBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


