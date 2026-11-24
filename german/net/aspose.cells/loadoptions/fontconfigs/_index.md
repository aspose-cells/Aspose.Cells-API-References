---
title: "LoadOptions.FontConfigs"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "LoadOptions-Eigenschaft. Ruft einzelne Schriftkonfigurationen ab und legt sie fest. Funktioniert nur für die Arbeitsmappe, die diese LoadOptions zum Laden verwendet."
type: docs
url: /de/net/aspose.cells/loadoptions/fontconfigs/
---
## LoadOptions.FontConfigs property

Ruft einzelne Schriftkonfigurationen ab und legt sie fest. Funktioniert nur für die [`Workbook`](../../workbook/), die diese [`LoadOptions`](../) zum Laden verwendet.

```csharp
public IndividualFontConfigs FontConfigs { get; set; }
```

### Beispiele

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyFontConfigsDemo
    {
        public static void Run()
        {
            // Ladeoptionen mit FontConfigs erstellen
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                FontConfigs = new IndividualFontConfigs()
            };

            // Legen Sie einige Schriftart-Ersetzungsregeln mit der richtigen API fest
            loadOptions.FontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman" });
            loadOptions.FontConfigs.SetFontSubstitutes("Courier New", new string[] { "Consolas" });

            // Lade eine CSV-Datei mit den angegebenen Optionen
            Workbook workbook = new Workbook("sample.csv", loadOptions);

            // Speichere die Arbeitsmappe in einer Excel‑Datei
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [IndividualFontConfigs](../../individualfontconfigs/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


