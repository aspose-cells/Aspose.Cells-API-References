---
title: "MsoLineFormat.IsVisible"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "MsoLineFormat-Eigenschaft. Gibt an, ob das Objekt sichtbar ist"
type: docs
url: /de/net/aspose.cells.drawing/msolineformat/isvisible/
---
## MsoLineFormat.IsVisible property

Gibt an, ob das Objekt sichtbar ist.

```csharp
public bool IsVisible { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge eine Rechteckform mit sichtbarem Rand hinzu
            var shape1 = worksheet.Shapes.AddRectangle(1, 0, 0, 100, 100, 100);
            shape1.LineFormat.IsVisible = true;

            // Füge eine Ovalform mit unsichtbarem Rand hinzu
            var shape2 = worksheet.Shapes.AddOval(2, 0, 150, 100, 100, 100);
            shape2.LineFormat.IsVisible = false;

            // Überprüfe und gib die Werte der IsVisible-Eigenschaft aus
            Console.WriteLine("Rectangle border visible: " + shape1.LineFormat.IsVisible);
            Console.WriteLine("Oval border visible: " + shape2.LineFormat.IsVisible);

            // Speichere die Arbeitsmappe
            workbook.Save("MsoLineFormat_IsVisible_Demo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


