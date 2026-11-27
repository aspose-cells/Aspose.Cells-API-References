---
title: "LoadOptions.FontConfigs"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions‑egenskap. Hämtar och anger individuella teckensnittskonfigurationer. Fungerar endast för den Workbook som använder dessa LoadOptions för att läsa in."
type: docs
url: /sv/net/aspose.cells/loadoptions/fontconfigs/
---
## LoadOptions.FontConfigs property

Hämtar och anger individuella teckensnittskonfigurationer. Fungerar endast för den [`Workbook`](../../workbook/) som använder dessa [`LoadOptions`](../) för att läsa in.

```csharp
public IndividualFontConfigs FontConfigs { get; set; }
```

### Exempel

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
            // Skapa laddningsalternativ med FontConfigs
            TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
            {
                FontConfigs = new IndividualFontConfigs()
            };

            // Ange några teckensnittssubstitutionsregler med rätt API
            loadOptions.FontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman" });
            loadOptions.FontConfigs.SetFontSubstitutes("Courier New", new string[] { "Consolas" });

            // Läs in en CSV-fil med de angivna alternativen
            Workbook workbook = new Workbook("sample.csv", loadOptions);

            // Spara arbetsboken till en Excel-fil
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [IndividualFontConfigs](../../individualfontconfigs/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


