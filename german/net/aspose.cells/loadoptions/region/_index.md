---
title: "LoadOptions.Region"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadOptions-Eigenschaft. Gibt die regionalen Einstellungen zurück, die für die zu ladende Arbeitsmappe verwendet werden, oder legt sie fest"
type: docs
url: /de/net/aspose.cells/loadoptions/region/
---
## LoadOptions.Region property

Liest oder legt die regionalen Einstellungen fest, die für die zu ladende Arbeitsmappe verwendet werden.

```csharp
public CountryCode Region { get; set; }
```

### Hinweise

Die regionalen Einstellungen können verwendet werden, um einige Funktionen für die Arbeitsmappe zu initialisieren, wie Schriftarten, Designs usw. Für textbasierte Dateiformate, wie CSV, HTML, ..., wird die regionale Einstellung auch verwendet, um Zahlenformate zu erkennen und Textwerte in numerische oder Datums‑Uhrzeit‑Werte für Zellen zu konvertieren. Diese Einstellung wird später für die instanzierte Arbeitsmappe beibehalten, das heißt, [`Region`](../../workbooksettings/region/) der Arbeitsmappe verwendet dieselbe Region mit dieser Eigenschaft.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyRegionDemo
    {
        public static void Run()
        {
            // Load-Optionen für HTML-Datei erstellen
            LoadOptions loadOpts = new LoadOptions(LoadFormat.Html);
            
            // Region auf USA setzen
            loadOpts.Region = CountryCode.USA;
            
            // HTML-Datei mit den angegebenen Regionseinstellungen laden
            Workbook wb = new Workbook("example.html", loadOpts);
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet ws = wb.Worksheets[0];
            
            // Region-spezifische Formatierung demonstrieren, indem der Stil einer Zelle geprüft wird
            Style style = ws.Cells["A1"].GetStyle();
            Console.WriteLine("Font used in cell A1: " + style.Font.Name);
            Console.WriteLine("Region used for loading: " + loadOpts.Region);
        }
    }
}
```

### Siehe auch

* enum [CountryCode](../../countrycode/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


