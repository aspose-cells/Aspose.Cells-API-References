---
title: "HtmlSaveOptions.EncodeEntityAsCode"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlSaveOptions property. Gibt an, ob HTML-Zeichenentitäten durch dezimale Codes ersetzt werden. z. B. wird nbsp durch 160 ersetzt. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells/htmlsaveoptions/encodeentityascode/
---
## HtmlSaveOptions.EncodeEntityAsCode property

Gibt an, ob die HTML‑Zeichenentitäten durch Dezimalcodes ersetzt werden. (z. B. "&amp;nbsp;" wird durch "&amp;#160;" ersetzt). Der Standardwert ist false.

```csharp
public bool EncodeEntityAsCode { get; set; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class HtmlSaveOptionsPropertyEncodeEntityAsCodeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge Beispieldaten mit Sonderzeichen hinzu
            worksheet.Cells["A1"].PutValue("Sample & Text");
            worksheet.Cells["A2"].PutValue("Another <Test> String");
            worksheet.Cells["A3"].PutValue("Price: $100");

            // HTML‑Speicheroptionen erstellen
            HtmlSaveOptions options = new HtmlSaveOptions();

            // Zeige den aktuellen Wert von EncodeEntityAsCode an
            Console.WriteLine("Current EncodeEntityAsCode value: " + options.EncodeEntityAsCode);

            // Setze EncodeEntityAsCode auf true
            options.EncodeEntityAsCode = true;

            // Speichern mit als Code codierten Entitäten
            workbook.Save("HtmlWithEncodedEntities.html", options);

            // Setze EncodeEntityAsCode auf false
            options.EncodeEntityAsCode = false;

            // Speichern mit Entitäten unverändert
            workbook.Save("HtmlWithRawEntities.html", options);

            // Vergleiche die Ausgabedateien
            Console.WriteLine("Files created:");
            Console.WriteLine("1. HtmlWithEncodedEntities.html - with encoded entities");
            Console.WriteLine("2. HtmlWithRawEntities.html - with raw entities");
        }
    }
}
```

### Siehe auch

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


