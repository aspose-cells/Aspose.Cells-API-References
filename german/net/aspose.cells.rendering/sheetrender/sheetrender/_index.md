---
title: "SheetRender.SheetRender"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SheetRender-Konstruktor. Der Aufbau von SheetRender benötigt ein Arbeitsblatt und ImageOrPrintOptions als Parameter"
type: docs
url: /de/net/aspose.cells.rendering/sheetrender/sheetrender/
---
## SheetRender constructor

Der Konstruktor von SheetRender benötigt ein Arbeitsblatt und ImageOrPrintOptions als Parameter

```csharp
public SheetRender(Worksheet worksheet, ImageOrPrintOptions options)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Arbeitsblatt | Arbeitsblatt | Geben Sie an, welche Tabelle gerendert werden soll. |
| Optionen | ImageOrPrintOptions | ImageOrPrintOptions enthält einige Eigenschaften des Ausgabebildes |

### Beispiele

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class SheetRenderMethodCtorWithWorksheetImageOrPrintOptionsDemo
    {
        public static void Run()
        {
            // Erstellen Sie ein Arbeitsbuch und fügen Sie einige Beispieldaten hinzu
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten zu Zellen hinzu
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["A3"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue(25);

            // Bild-/Druckoptionen erstellen
            ImageOrPrintOptions options = new ImageOrPrintOptions();
            options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
            options.OnePagePerSheet = true;

            // Erstellen Sie SheetRender mit Worksheet und ImageOrPrintOptions
            SheetRender render = new SheetRender(worksheet, options);

            // Seitenanzahl ausgeben
            Console.WriteLine("Page count: " + render.PageCount);

            // Speichern Sie das gerenderte Bild
            render.ToImage(0, "output.png");
        }
    }
}
```

### Siehe auch

* class [Worksheet](../../../aspose.cells/worksheet/)
* class [ImageOrPrintOptions](../../imageorprintoptions/)
* class [SheetRender](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)


