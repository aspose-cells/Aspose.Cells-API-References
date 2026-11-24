---
title: "LoadOptions.CultureInfo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadOptions-Eigenschaft. Gibt die regionalen Einstellungen zurück, die für die zu ladende Arbeitsmappe verwendet werden, oder legt sie fest"
type: docs
url: /de/net/aspose.cells/loadoptions/cultureinfo/
---
## LoadOptions.CultureInfo property

Liest oder legt die regionalen Einstellungen fest, die für die zu ladende Arbeitsmappe verwendet werden.

```csharp
public CultureInfo CultureInfo { get; set; }
```

### Hinweise

Diese Eigenschaft hat die gleiche Wirkung wie [`Region`](../region/) zum Festlegen regionaler Einstellungen.

### Beispiele

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyCultureInfoDemo
    {
        public static void Run()
        {
            // Beispiel‑Excel‑Datei erstellen
            Workbook sampleWorkbook = new Workbook();
            sampleWorkbook.Worksheets[0].Cells["A1"].PutValue(1234.56);
            sampleWorkbook.Save("sample.xlsx", SaveFormat.Xlsx);

            // Mit spezifischer Kultur laden
            LoadOptions options = new LoadOptions(LoadFormat.Xlsx);
            options.CultureInfo = new CultureInfo("de-DE"); // German culture uses comma as decimal separator
            
            Workbook workbook = new Workbook("sample.xlsx", options);
            Console.WriteLine("Value with German culture: " + workbook.Worksheets[0].Cells["A1"].StringValue);
        }
    }
}
```

### Siehe auch

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


