---
title: "HtmlSaveOptions.AddGenericFont"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob eine generische Schriftart zur CSS-Schriftfamilie hinzugefügt wird. Der Standardwert ist true"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/addgenericfont/
---
## HtmlSaveOptions.AddGenericFont property

Gibt an, ob eine generische Schriftart zur CSS‑font-family hinzugefügt werden soll. Der Standardwert ist true

```csharp
public bool AddGenericFont { get; set; }
```

### Beispiele

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyAddGenericFontDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Beispieltext mit einer bestimmten Schriftart festlegen
            var cell = worksheet.Cells["A1"];
            cell.PutValue("Sample Text");
            Style style = cell.GetStyle();
            style.Font.Name = "Pacifico";
            cell.SetStyle(style);

            // Speichern mit aktiviertem AddGenericFont (Standard)
            HtmlSaveOptions options = new HtmlSaveOptions(SaveFormat.Html);
            workbook.Save("output_with_generic.html", options);

            // Speichern mit deaktiviertem AddGenericFont
            options.AddGenericFont = false;
            workbook.Save("output_without_generic.html", options);

            // Ergebnisse überprüfen.
            string withGeneric = File.ReadAllText("output_with_generic.html");
            string withoutGeneric = File.ReadAllText("output_without_generic.html");

            Console.WriteLine("With generic font: " + (withGeneric.Contains("font-family:Pacifico,sans-serif") ? "Found" : "Not found"));
            Console.WriteLine("Without generic font: " + (withoutGeneric.Contains("font-family:Pacifico,sans-serif") ? "Found" : "Not found"));
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


