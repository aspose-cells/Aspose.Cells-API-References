---
title: "HtmlLoadOptions.AutoFitColsAndRows"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlLoadOptions-Eigenschaft. Gibt an, ob Spalten und Zeilen automatisch angepasst werden. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells/htmlloadoptions/autofitcolsandrows/
---
## HtmlLoadOptions.AutoFitColsAndRows property

Gibt an, ob Spalten und Zeilen automatisch angepasst werden. Der Standardwert ist false.

```csharp
public bool AutoFitColsAndRows { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyAutoFitColsAndRowsDemo
    {
        public static void Run()
        {
            // HTML-Ladeoptionen erstellen
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            
            // Automatisches Anpassen von Spalten und Zeilen aktivieren
            loadOptions.AutoFitColsAndRows = true;
            
            // HTML-Datei mit den angegebenen Optionen laden
            Workbook workbook = new Workbook("example.html", loadOptions);
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Automatisches Anpassen von Spalten und Zeilen wird beim Laden angewendet
            Console.WriteLine("Columns and rows have been auto-fitted during HTML import.");
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


