---
title: "Worksheet.RemoveAllDrawingObjects"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Worksheet method. Tar bort alla ritobjekt i detta worksheet"
type: docs
url: /sv/net/aspose.cells/worksheet/removealldrawingobjects/
---
## Worksheet.RemoveAllDrawingObjects method

Tar bort alla ritobjekt i detta kalkylblad.

```csharp
public void RemoveAllDrawingObjects()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRemoveAllDrawingObjectsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Lägg till några ritobjekt i worksheet
            worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 50);
            worksheet.Shapes.AddLine(1, 0, 5, 100, 5, 150);
            
            // Spara innan du tar bort objekt
            workbook.Save("BeforeRemove.xlsx", SaveFormat.Xlsx);
            
            // Ta bort alla ritobjekt
            worksheet.RemoveAllDrawingObjects();
            
            // Spara efter att ha tagit bort objekt
            workbook.Save("AfterRemove.xlsx", SaveFormat.Xlsx);
            
            // Frigör arbetsboken
            workbook.Dispose();
        }
    }
}
```

### Se även

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


