---
title: "TxtSaveOptions.FormatStrategy"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "TxtSaveOptions-Eigenschaft. Liest und setzt die Formatstrategie beim Exportieren des Zellwerts als Zeichenkette"
type: docs
url: /de/net/aspose.cells/txtsaveoptions/formatstrategy/
---
## TxtSaveOptions.FormatStrategy property

Liest und setzt die Formatstrategie beim Export des Zellenwerts als Zeichenkette.

```csharp
public CellValueFormatStrategy FormatStrategy { get; set; }
```

### Beispiele

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class TxtSaveOptionsPropertyFormatStrategyDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Werte mit unterschiedlichen Formaten festlegen
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Laptop");
            worksheet.Cells["B2"].PutValue(999.99);
            worksheet.Cells["A3"].PutValue("Phone");
            worksheet.Cells["B3"].PutValue(599.99);

            // Zahlenformat auf Preise anwenden
            Style style = workbook.CreateStyle();
            style.Number = 2; // Format as currency
            worksheet.Cells["B2:B3"].SetStyle(style);

            // Text‑Speicheroptionen mit verschiedenen Formatstrategien konfigurieren
            TxtSaveOptions options = new TxtSaveOptions
            {
                Separator = '\t',
                FormatStrategy = CellValueFormatStrategy.DisplayStyle // Show formatted values
            };

            // Speichern mit Anzeigeformatierung
            workbook.Save("FormattedOutput.txt", options);

            // Auf keine Formatstrategie umstellen
            options.FormatStrategy = CellValueFormatStrategy.None;
            workbook.Save("RawOutput.txt", options);

            Console.WriteLine("Files saved with different format strategies.");
        }
    }
}
```

### Siehe auch

* enum [CellValueFormatStrategy](../../cellvalueformatstrategy/)
* class [TxtSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


