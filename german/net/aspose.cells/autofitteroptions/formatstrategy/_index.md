---
title: "AutoFitterOptions.FormatStrategy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "AutoFitterOptions-Eigenschaft. Gibt die Formatierungsstrategie zurück oder legt sie fest"
type: docs
url: /de/net/aspose.cells/autofitteroptions/formatstrategy/
---
## AutoFitterOptions.FormatStrategy property

Liest und setzt die formatierte Strategie.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Hinweise

Der Standardwert ist CellStyle für die Leistung.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class AutoFitterOptionsPropertyFormatStrategyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Beispieldaten festlegen und Text umbrechen
            worksheet.Cells["A1"].PutValue("Sample text for FormatStrategy demo");
            Style style = worksheet.Cells["A1"].GetStyle();
            style.IsTextWrapped = true;
            worksheet.Cells["A1"].SetStyle(style);

            // Erstelle AutoFitterOptions mit FormatStrategy
            AutoFitterOptions options = new AutoFitterOptions
            {
                FormatStrategy = CellValueFormatStrategy.DisplayString,
                AutoFitMergedCellsType = AutoFitMergedCellsType.EachLine
            };

            // Wende Auto-Fit mit den angegebenen Optionen an
            worksheet.AutoFitRows(options);

            // Ergebnis speichern
            workbook.Save("FormatStrategyDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [AutoFitterOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


