---
title: "NoneBulletValue.Type"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Свойство NoneBulletValue. Возвращает тип значения маркера"
type: docs
url: /ru/net/aspose.cells.drawing.texts/nonebulletvalue/type/
---
## NoneBulletValue.Type property

Получает тип значения маркера.

```csharp
public override BulletType Type { get; }
```

### Примеры

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

### См. также

* enum [BulletType](../../bullettype/)
* class [NoneBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


