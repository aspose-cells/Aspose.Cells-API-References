---
title: "LoadOptions.AutoFitterOptions"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadOptions-Eigenschaft. Liest und setzt die Auto-Fitter-Optionen"
type: docs
url: /de/net/aspose.cells/loadoptions/autofitteroptions/
---
## LoadOptions.AutoFitterOptions property

Liest und legt die Auto‑Fitter‑Optionen fest

```csharp
public AutoFitterOptions AutoFitterOptions { get; set; }
```

### Hinweise

Nur jetzt für xlsx- und SpreadsheetML-Dateien.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyAutoFitterOptionsDemo
    {
        public static void Run()
        {
            // AutoFitterOptions erstellen und Eigenschaften setzen
            AutoFitterOptions options = new AutoFitterOptions();
            options.AutoFitMergedCells = true;
            options.OnlyAuto = false;

            // Erstelle LoadOptions und weise AutoFitterOptions zu
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.AutoFitterOptions = options;

            // Arbeitsmappe mit den angegebenen Optionen laden
            Workbook workbook = new Workbook("example.xlsx", loadOptions);

            // Demonstriere automatisches Anpassen, indem du die Zeilenhöhe ermittelst
            double rowHeight = workbook.Worksheets[0].Cells.GetRowHeight(0);
            Console.WriteLine("Row height after auto-fitting: " + rowHeight);
        }
    }
}
```

### Siehe auch

* class [AutoFitterOptions](../../autofitteroptions/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


