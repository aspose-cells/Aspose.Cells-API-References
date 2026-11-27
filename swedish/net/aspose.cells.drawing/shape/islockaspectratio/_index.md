---
title: "Shape.IsLockAspectRatio"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. True betyder att bildförhållandet för formen är låst"
type: docs
url: /sv/net/aspose.cells.drawing/shape/islockaspectratio/
---
## Shape.IsLockAspectRatio property

Sant betyder att bildförhållandet för formen är låst.

```csharp
[Obsolete("Use Shape.IsAspectRatioLocked property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IsLockAspectRatio { get; set; }
```

### Anmärkningar

Endast för bilder och Ole-objekt. OBS: Denna medlem är nu föråldrad. Använd istället Shape.IsAspectRatioLocked-egenskapen. Denna egenskap kommer att tas bort 12 månader senare från och med juli 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyIsLockAspectRatioDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en rektangel med alla nödvändiga parametrar
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 200, 0);

            // Lås bildförhållande
            shape.IsLockAspectRatio = true;
            Console.WriteLine("Aspect ratio locked: " + shape.IsLockAspectRatio);

            // Lås upp bildförhållande
            shape.IsLockAspectRatio = false;
            Console.WriteLine("Aspect ratio locked: " + shape.IsLockAspectRatio);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


