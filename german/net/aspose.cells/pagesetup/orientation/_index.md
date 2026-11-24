---
title: "PageSetup.Orientation"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt die Druckorientierung der Seite an"
type: docs
url: /de/net/aspose.cells/pagesetup/orientation/
---
## PageSetup.Orientation property

Stellt die Druckorientierung der Seite dar.

```csharp
public PageOrientationType Orientation { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyOrientationDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Setze die Seitenorientierung auf Querformat
            worksheet.PageSetup.Orientation = PageOrientationType.Landscape;
            
            // Füge einige Beispieldaten hinzu, um die Wirkung zu demonstrieren
            worksheet.Cells["A1"].PutValue("Landscape Orientation Demo");
            for (int i = 1; i <= 10; i++)
            {
                worksheet.Cells[$"A{i}"].PutValue($"Data Row {i}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("PageOrientationDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Siehe auch

* enum [PageOrientationType](../../pageorientationtype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


