---
title: "HtmlSaveOptions.DisableCss"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt an, ob nur Inline-Stile angewendet werden, ohne CSS zu verwenden. Der Standardwert ist false."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/disablecss/
---
## HtmlSaveOptions.DisableCss property

Gibt an, ob nur Inline‑Stile angewendet werden, ohne sich auf CSS zu verlassen. Der Standardwert ist false.

```csharp
public bool DisableCss { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HtmlSaveOptionsPropertyDisableCssDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten und Formatierung hinzu
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A1"].GetStyle().Font.IsBold = true;
            worksheet.Cells["A1"].GetStyle().Font.Color = System.Drawing.Color.Red;
            worksheet.Cells["B1"].PutValue("Formatted Cell");
            worksheet.Cells["B1"].GetStyle().Font.IsItalic = true;
            worksheet.Cells["B1"].GetStyle().Font.Underline = FontUnderlineType.Single;

            // Erstelle eine HtmlSaveOptions-Instanz
            HtmlSaveOptions options = new HtmlSaveOptions();

            // Zeige den aktuellen DisableCss-Wert an
            Console.WriteLine("Current DisableCss value: " + options.DisableCss);

            // Setze DisableCss auf true (unter Verwendung von Inline-Stilen anstelle von CSS)
            options.DisableCss = true;
            workbook.Save("HtmlWithInlineStyles.html", options);

            // Setze DisableCss auf false (unter Verwendung von CSS-Stilen)
            options.DisableCss = false;
            workbook.Save("HtmlWithCssStyles.html", options);

            // Vergleiche die Ausgabedateien, um den Unterschied im Styling-Ansatz zu sehen
            Console.WriteLine("Files saved with different DisableCss settings.");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


