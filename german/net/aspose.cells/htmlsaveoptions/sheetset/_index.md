---
title: "HtmlSaveOptions.SheetSet"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions property. Ruft die zu rendernden Arbeitsblätter ab oder legt sie fest. Standard ist alle sichtbaren Arbeitsblätter in der Arbeitsmappe Visible"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/sheetset/
---
## HtmlSaveOptions.SheetSet property

Ruft die zu rendernden Arbeitsblätter ab oder legt sie fest. Standard ist alle sichtbaren Arbeitsblätter in der Arbeitsmappe: [`Visible`](../../../aspose.cells.rendering/sheetset/visible/).

```csharp
public SheetSet SheetSet { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Rendering;
    using System;

    public class HtmlSaveOptionsPropertySheetSetDemo
    {
        public static void Run()
        {
            // Eine neue Arbeitsmappe mit mehreren Arbeitsblättern erstellen
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");
            
            // Ein Blatt zur Demonstration ausblenden
            workbook.Worksheets[1].IsVisible = false;

            // Einige Beispieldaten in jedem Blatt festlegen
            for (int i = 0; i < workbook.Worksheets.Count; i++)
            {
                Worksheet sheet = workbook.Worksheets[i];
                sheet.Cells["A1"].PutValue($"Data from {sheet.Name}");
            }

            // Erstelle eine HtmlSaveOptions-Instanz
            HtmlSaveOptions options = new HtmlSaveOptions();

            // Aktuellen SheetSet-Wert anzeigen (Standard ist null, was alle sichtbaren Blätter bedeutet)
            Console.WriteLine("Current SheetSet value: " + (options.SheetSet == null ? "All visible sheets" : "Custom set"));

            // SheetSet so festlegen, dass nur bestimmte Blätter (nach Index) enthalten sind
            options.SheetSet = new SheetSet(new int[] { 0, 2 });

            // Als HTML speichern – nur die angegebenen Blätter werden eingeschlossen
            workbook.Save("HtmlWithCustomSheetSet.html", options);

            // SheetSet ändern, sodass nur sichtbare Blätter enthalten sind
            options.SheetSet = SheetSet.Visible;
            workbook.Save("HtmlWithVisibleSheets.html", options);

            // SheetSet ändern, sodass nur das aktive Blatt enthalten ist
            workbook.Worksheets[2].IsSelected = true; // Activate the sheet by selecting it
            options.SheetSet = SheetSet.Active;
            workbook.Save("HtmlWithActiveSheet.html", options);
        }
    }
}
```

### Siehe auch

* class [SheetSet](../../../aspose.cells.rendering/sheetset/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


