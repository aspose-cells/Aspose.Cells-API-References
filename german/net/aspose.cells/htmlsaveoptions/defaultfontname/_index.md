---
title: "HtmlSaveOptions.DefaultFontName"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions-Eigenschaft. Gibt den Standard-Schriftartnamen für den HTML-Export an. Die Standardschriftart wird verwendet, wenn die Schriftart des Stils nicht vorhanden ist. Ist diese Eigenschaft null, verwendet Aspose.Cells eine universelle Schriftart, die dieselbe Familie wie die Originalschriftart hat. Der Standardwert ist null."
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/defaultfontname/
---
## HtmlSaveOptions.DefaultFontName property

Gib den Standard‑Schriftartnamen für den Export von HTML an, die Standardschriftart wird verwendet, wenn die Schriftart des Stils nicht vorhanden ist. Ist diese Eigenschaft null, verwendet Aspose.Cells eine universelle Schriftart, die dieselbe Familie wie die Originalschriftart hat. Der Standardwert ist null.

```csharp
public string DefaultFontName { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyDefaultFontNameDemo
    {
        public static void Run()
        {
            // Erstelle ein Beispielarbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["A1"].PutValue("Sample Text");
            
            // HTML-Speicheroptionen mit benutzerdefinierter Standardschriftart festlegen
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.DefaultFontName = "Courier New";
            
            // In HTML mit der angegebenen Schriftart speichern
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file saved with default font: " + saveOptions.DefaultFontName);
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


