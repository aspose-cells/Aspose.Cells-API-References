---
title: "Worksheet.RemoveAllDrawingObjects"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Entfernt alle Zeichenobjekte in diesem Arbeitsblatt"
type: docs
url: /de/net/aspose.cells/worksheet/removealldrawingobjects/
---
## Worksheet.RemoveAllDrawingObjects method

Entfernt alle Zeichenobjekte in diesem Arbeitsblatt.

```csharp
public void RemoveAllDrawingObjects()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodRemoveAllDrawingObjectsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einige Zeichenobjekte zum Worksheet hinzu
            worksheet.Shapes.AddRectangle(1, 0, 1, 100, 100, 50);
            worksheet.Shapes.AddLine(1, 0, 5, 100, 5, 150);
            
            // Speichere vor dem Entfernen der Objekte
            workbook.Save("BeforeRemove.xlsx", SaveFormat.Xlsx);
            
            // Entferne alle Zeichenobjekte
            worksheet.RemoveAllDrawingObjects();
            
            // Speichere nach dem Entfernen der Objekte
            workbook.Save("AfterRemove.xlsx", SaveFormat.Xlsx);
            
            // Arbeitsmappe freigeben
            workbook.Dispose();
        }
    }
}
```

### Siehe auch

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


