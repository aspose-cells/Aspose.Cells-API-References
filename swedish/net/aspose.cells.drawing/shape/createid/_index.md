---
title: "Shape.CreateId"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Shape-egenskap. Hämtar och anger create id för denna form"
type: docs
url: /sv/net/aspose.cells.drawing/shape/createid/
---
## Shape.CreateId property

Hämtar och anger skapande-ID för denna form.

```csharp
public Guid CreateId { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapePropertyCreateIdDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till en rektangelform
            Shape shape = worksheet.Shapes.AddRectangle(10, 10, 100, 100, 200, 150);
            
            // Skapa och tilldela ett nytt GUID som CreateId
            Guid createId = Guid.NewGuid();
            shape.CreateId = createId;
            
            // Spara arbetsboken
            workbook.Save("ShapeCreateIdDemo.xlsx");
            
            // Läs in arbetsboken igen för att verifiera att CreateId kvarstår
            Workbook loadedWorkbook = new Workbook("ShapeCreateIdDemo.xlsx");
            Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
            
            // Skriv ut CreateId för verifiering
            Console.WriteLine("Original CreateId: " + createId);
            Console.WriteLine("Loaded CreateId: " + loadedShape.CreateId);
        }
    }
}
```

### Se även

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


