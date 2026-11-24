---
title: "HtmlSaveOptions.HiddenColDisplayType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Versteckte Spalte – die Breite dieser Spalte ist in Excel 0. Vor dem Speichern in das HTML-Format, wenn HtmlHiddenColDisplayType auf Remove gesetzt ist, wird die versteckte Spalte nicht ausgegeben; wenn der Wert Hidden ist, wird die Spalte ausgegeben, aber versteckt. Der Standardwert ist Hidden."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/hiddencoldisplaytype/
---
## HtmlSaveOptions.HiddenColDisplayType property

Versteckte Spalte (die Breite dieser Spalte ist 0) in Excel, bevor sie in das HTML‑Format gespeichert wird: Wenn HtmlHiddenColDisplayType "Remove" ist, wird die versteckte Spalte nicht ausgegeben; ist der Wert "Hidden", wird die Spalte ausgegeben, aber verborgen. Der Standardwert ist "Hidden".

```csharp
public HtmlHiddenColDisplayType HiddenColDisplayType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHiddenColDisplayTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Spalte C ausblenden (Index 2)
            worksheet.Cells.HideColumn(2);

            // Füge einige Daten zur Demonstration hinzu
            worksheet.Cells["A1"].PutValue("Visible Column A");
            worksheet.Cells["B1"].PutValue("Visible Column B");
            worksheet.Cells["C1"].PutValue("Hidden Column C");
            worksheet.Cells["D1"].PutValue("Visible Column D");

            // HTML-Speicheroptionen mit unterschiedlichen HiddenColDisplayType-Einstellungen erstellen
            HtmlSaveOptions optionsRemove = new HtmlSaveOptions
            {
                HiddenColDisplayType = HtmlHiddenColDisplayType.Remove
            };

            HtmlSaveOptions optionsHidden = new HtmlSaveOptions
            {
                HiddenColDisplayType = HtmlHiddenColDisplayType.Hidden
            };

            // Mit verschiedenen Optionen speichern
            workbook.Save("output_remove.html", optionsRemove); // Column C will be removed
            workbook.Save("output_hidden.html", optionsHidden); // Column C will be hidden but space preserved
        }
    }
}
```

### Siehe auch

* enum [HtmlHiddenColDisplayType](../../htmlhiddencoldisplaytype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


