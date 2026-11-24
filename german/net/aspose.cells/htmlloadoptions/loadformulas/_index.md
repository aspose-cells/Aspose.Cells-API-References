---
title: "HtmlLoadOptions.LoadFormulas"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HtmlLoadOptions-Eigenschaft. Gibt an, ob Formeln importiert werden, wenn die ursprüngliche HTML-Datei Formeln enthält"
type: docs
url: /de/net/aspose.cells/htmlloadoptions/loadformulas/
---
## HtmlLoadOptions.LoadFormulas property

Gibt an, ob Formeln importiert werden, wenn die ursprüngliche HTML‑Datei Formeln enthält

```csharp
public bool LoadFormulas { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyLoadFormulasDemo
    {
        public static void Run()
        {
            // Erstelle eine Instanz von HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // Setze LoadFormulas auf true, um Formeln aus HTML zu laden
            loadOptions.LoadFormulas = true;

            // Eine HTML-Datei, die Formeln enthält, in eine Arbeitsmappe laden
            Workbook workbook = new Workbook("input.html", loadOptions);

            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];

            // Formel aus Zelle A1 anzeigen (falls in HTML vorhanden)
            Console.WriteLine("Formula in A1: " + worksheet.Cells["A1"].Formula);

            // Speichere die Arbeitsmappe in einer Excel‑Datei
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


