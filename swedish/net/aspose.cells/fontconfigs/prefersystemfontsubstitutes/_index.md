---
title: "FontConfigs.PreferSystemFontSubstitutes"
second_title: "Aspose.Cells för .NET API‑referens"
description: "FontConfigs-egenskapen. Anger om systemteckensnittssubstitut ska användas först eller inte när ett teckensnitt inte finns och substitutet för detta teckensnitt inte är angivet. t.ex. På Ubuntu ersätts Arial vanligtvis av Liberation Sans. Standardvärdet är false"
type: docs
url: /sv/net/aspose.cells/fontconfigs/prefersystemfontsubstitutes/
---
## FontConfigs.PreferSystemFontSubstitutes property

Indikera om systemets teckensnittssubstitut ska användas först eller inte när ett teckensnitt inte finns tillgängligt och substitutet för detta teckensnitt inte är angivet. t.ex. På Ubuntu ersätts teckensnittet \"Arial\" vanligtvis av \"Liberation Sans\". Standardvärdet är falskt.

```csharp
public static bool PreferSystemFontSubstitutes { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class FontConfigsPropertyPreferSystemFontSubstitutesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Visa aktuellt värde för PreferSystemFontSubstitutes
            Console.WriteLine("Current PreferSystemFontSubstitutes value: " + FontConfigs.PreferSystemFontSubstitutes);

            // Ställ in PreferSystemFontSubstitutes till true
            FontConfigs.PreferSystemFontSubstitutes = true;
            Console.WriteLine("PreferSystemFontSubstitutes set to: " + FontConfigs.PreferSystemFontSubstitutes);

            // Skapa en cell med ett teckensnitt som kan behöva ersättning
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Text with Arial font");
            Style style = cell.GetStyle();
            style.Font.Name = "Arial";
            cell.SetStyle(style);

            // Spara arbetsboken för att se effekterna av teckensnittsersättning
            workbook.Save("FontSubstitutionDemo.xlsx");

            // Återställ till standardvärde
            FontConfigs.PreferSystemFontSubstitutes = false;
            Console.WriteLine("PreferSystemFontSubstitutes reset to: " + FontConfigs.PreferSystemFontSubstitutes);
        }
    }
}
```

### Se även

* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


