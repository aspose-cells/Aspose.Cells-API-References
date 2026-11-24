---
title: "HtmlSaveOptions.HtmlVersion"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions property. Gibt die Version des HTML-Standards an, die beim Speichern im HTML-Format verwendet werden soll. Der Standardwert ist HtmlVersion.Default"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/htmlversion/
---
## HtmlSaveOptions.HtmlVersion property

Gibt die HTML‑Standardversion an, die beim Speichern im HTML‑Format verwendet werden soll. Der Standardwert ist HtmlVersion.Default.

```csharp
public HtmlVersion HtmlVersion { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsPropertyHtmlVersionDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie einige Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("HTML Version Demo");
            worksheet.Cells["A2"].PutValue("This demonstrates HtmlVersion property");
            worksheet.Cells["B3"].PutValue(123.45);
            worksheet.Cells["C4"].PutValue("Sample Text");
            
            // Erstelle eine HtmlSaveOptions-Instanz
            HtmlSaveOptions options = new HtmlSaveOptions();
            
            // Zeige den aktuellen HtmlVersion-Wert an
            Console.WriteLine("Current HtmlVersion: " + options.HtmlVersion);
            
            // Setze HtmlVersion auf HTML5
            options.HtmlVersion = HtmlVersion.Html5;
            Console.WriteLine("HtmlVersion changed to: " + options.HtmlVersion);
            
            // Speichern mit HTML5-Version
            workbook.Save("HtmlVersion_Html5.html", options);
            
            // Wechsel zu XHTML
            options.HtmlVersion = HtmlVersion.XHtml;
            Console.WriteLine("HtmlVersion changed to: " + options.HtmlVersion);
            
            // Speichern mit XHTML-Version
            workbook.Save("HtmlVersion_XHtml.html", options);
            
            // Auf Standard zurücksetzen
            options.HtmlVersion = HtmlVersion.Default;
            Console.WriteLine("HtmlVersion reset to: " + options.HtmlVersion);
            
            // Speichern mit Standardversion
            workbook.Save("HtmlVersion_Default.html", options);
        }
    }
}
```

### Siehe auch

* enum [HtmlVersion](../../htmlversion/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


