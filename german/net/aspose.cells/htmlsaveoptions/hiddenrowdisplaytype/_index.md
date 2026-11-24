---
title: "HtmlSaveOptions.HiddenRowDisplayType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Versteckte Zeile – die Höhe dieser Zeile ist in Excel 0. Vor dem Speichern im HTML-Format, wenn HtmlHiddenRowDisplayType auf Remove gesetzt ist, wird die versteckte Zeile nicht ausgegeben; ist der Wert Hidden, wird die Zeile ausgegeben, aber als versteckt. Der Standardwert ist Hidden."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/hiddenrowdisplaytype/
---
## HtmlSaveOptions.HiddenRowDisplayType property

Versteckte Zeile (die Höhe dieser Zeile ist 0) in Excel, bevor sie in das HTML‑Format gespeichert wird: Wenn HtmlHiddenRowDisplayType "Remove" ist, wird die versteckte Zeile nicht ausgegeben; ist der Wert "Hidden", wird die Zeile ausgegeben, aber verborgen. Der Standardwert ist "Hidden".

```csharp
public HtmlHiddenRowDisplayType HiddenRowDisplayType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHiddenRowDisplayTypeDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten hinzu und verstecke eine Zeile
            worksheet.Cells["A1"].PutValue("Visible Row");
            worksheet.Cells["A2"].PutValue("Hidden Row");
            worksheet.Cells["A3"].PutValue("Visible Row");
            worksheet.Cells.HideRow(1); // Hide row 2 (0-based index 1)

            // Setze HTML-Speicheroptionen mit HiddenRowDisplayType
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.HiddenRowDisplayType = HtmlHiddenRowDisplayType.Hidden;

            // Als HTML speichern
            workbook.Save("output.html", options);

            Console.WriteLine("HTML file saved with hidden rows handled according to HiddenRowDisplayType setting.");
        }
    }
}
```

### Siehe auch

* enum [HtmlHiddenRowDisplayType](../../htmlhiddenrowdisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


