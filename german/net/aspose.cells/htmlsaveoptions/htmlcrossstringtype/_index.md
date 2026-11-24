---
title: "HtmlSaveOptions.HtmlCrossStringType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob ein Crosscell‑String beim Speichern einer Excel‑Datei im HTML‑Format auf dieselbe Weise wie in MS Excel angezeigt wird. Standardmäßig ist der Wert Default, sodass es bei Crosscell‑Strings nur geringe Unterschiede zwischen den von Aspose.Cells und MS Excel erstellten HTML‑Dateien gibt. Die Leistung beim Erstellen großer HTML‑Dateien ist jedoch mehrere Male höher, wenn der Wert auf Cross gesetzt wird, im Vergleich zu Default oder Fit2Cell."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/htmlcrossstringtype/
---
## HtmlSaveOptions.HtmlCrossStringType property

Gibt an, ob ein über mehrere Zellen erstreckender Text beim Speichern einer Excel‑Datei im HTML‑Format auf dieselbe Weise wie MS Excel angezeigt wird. Standardmäßig ist der Wert Default, sodass bei übergreifenden Zeichenketten nur geringe Unterschiede zwischen den von Aspose.Cells und MS Excel erzeugten HTML‑Dateien bestehen. Für die Erstellung großer HTML‑Dateien ist die Leistung jedoch mehrere Male höher, wenn der Wert auf Cross gesetzt wird, im Vergleich zu Default oder Fit2Cell.

```csharp
public HtmlCrossType HtmlCrossStringType { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHtmlCrossStringTypeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge Beispieldaten hinzu, die das Verhalten von Cross‑Strings demonstrieren
            worksheet.Cells["A1"].PutValue("Left Content");
            worksheet.Cells["B1"].PutValue("Right Content");
            
            // Abrufen und Ändern von Zellenstilen
            Style styleA1 = worksheet.Cells["A1"].GetStyle();
            styleA1.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            worksheet.Cells["A1"].SetStyle(styleA1);
            
            Style styleB1 = worksheet.Cells["B1"].GetStyle();
            styleB1.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            worksheet.Cells["B1"].SetStyle(styleB1);

            // HTML-Speicheroptionen konfigurieren
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.HtmlCrossStringType = HtmlCrossType.CrossHideRight;

            // Arbeitsmappe nach HTML speichern
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with CrossHideRight option.");
        }
    }
}
```

### Siehe auch

* enum [HtmlCrossType](../../htmlcrosstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


