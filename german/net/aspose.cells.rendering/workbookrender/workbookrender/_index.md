---
title: "WorkbookRender.WorkbookRender"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "WorkbookRender-Konstruktor. Die Konstruktion von WorkbookRender"
type: docs
url: /de/net/aspose.cells.rendering/workbookrender/workbookrender/
---
## WorkbookRender constructor

Der Aufbau von WorkbookRender

```csharp
public WorkbookRender(Workbook workbook, ImageOrPrintOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Arbeitsmappe | Arbeitsmappe | Geben Sie an, welche Arbeitsmappe gerendert werden soll. |
| Optionen | ImageOrPrintOptions | ImageOrPrintOptions enthält einige Eigenschaften des Ausgabebildes |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class WorkbookRenderMethodctorWithWorkbookImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Hello");
            worksheet.Cells["B1"].PutValue("World");
            
            // Bild-/Druckoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            
            // Arbeitsmappen-Renderer erstellen
            WorkbookRender renderer = new WorkbookRender(workbook, options);
            
            // Seitenanzahl ausgeben
            Console.WriteLine("Total pages: " + renderer.PageCount);
        }
    }
}
```

### Siehe auch

* class [Workbook](../../../aspose.cells/workbook/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [WorkbookRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


