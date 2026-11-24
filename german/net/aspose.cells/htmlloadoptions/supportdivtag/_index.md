---
title: "HtmlLoadOptions.SupportDivTag"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlLoadOptions-Eigenschaft. Gibt an, ob das Layout des div-Tags unterstützt wird, wenn die HTML-Datei es enthält. Der Standardwert ist false"
type: docs
url: /de/net/aspose.cells/htmlloadoptions/supportdivtag/
---
## HtmlLoadOptions.SupportDivTag property

Gibt an, ob das Layout des `<div>`‑Tags unterstützt wird, wenn die HTML‑Datei es enthält. Der Standardwert ist false.

```csharp
public bool SupportDivTag { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertySupportDivTagDemo
    {
        public static void Run()
        {
            // HTML-Ladeoptionen mit aktiviertem SupportDivTag erstellen
            HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions(LoadFormat.Html);
            htmlLoadOptions.SupportDivTag = true;

            // HTML-Datei mit div-Tags laden
            Workbook workbook = new Workbook("input.html", htmlLoadOptions);

            // Daten aus dem ersten Arbeitsblatt abrufen
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // Zellwert- und Stilinformationen ausgeben
            Console.WriteLine("Cell A1 value: " + cell.StringValue);
            Console.WriteLine("Is bold: " + cell.GetStyle().Font.IsBold);

            // Als Excel-Datei speichern
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


