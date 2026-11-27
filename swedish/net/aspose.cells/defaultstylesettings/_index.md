---
title: "Class DefaultStyleSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.DefaultStyleSettings-klass. Inställningar för standardvärdena för arbetsbokens stilegenskaper"
type: docs
url: /sv/net/aspose.cells/defaultstylesettings/
---
## DefaultStyleSettings class

Inställningar för standardvärdena för arbetsbokens stilegenskaper.

```csharp
public class DefaultStyleSettings
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [BuiltInPreference](../../aspose.cells/defaultstylesettings/builtinpreference/) { get; set; } | Indikerar om egenskapen för talformat är att föredra när stilen definierar både inbyggt talformat och anpassat mönster. Standardvärdet är false, vilket betyder att standardmässigt kommer det anpassade mönstret att användas för att formatera värden så länge det inte är tomt för en stil. |
| [FontName](../../aspose.cells/defaultstylesettings/fontname/) { get; set; } | Hämtar/Anger standardtypsnittets namn för arbetsboken |
| [FontSize](../../aspose.cells/defaultstylesettings/fontsize/) { get; set; } | Hämtar/Anger standardstorleken för standardtypsnittet i arbetsboken. |
| [HorizontalAlignment](../../aspose.cells/defaultstylesettings/horizontalalignment/) { get; set; } | Hämtar/Anger standardvärdet för horisontell justering |
| [VerticalAlignment](../../aspose.cells/defaultstylesettings/verticalalignment/) { get; set; } | Hämtar/Anger standardvärdet för vertikal justering |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class DefaultStyleSettingsDemo
    {
        public static void DefaultStyleSettingsExample()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till standardstilinställningarna för arbetsboken
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // Ställa in egenskaper
            defaultStyleSettings.BuiltInPreference = false;
            defaultStyleSettings.FontName = "Arial";
            defaultStyleSettings.FontSize = 12.0;
            defaultStyleSettings.HorizontalAlignment = TextAlignmentType.Center;
            defaultStyleSettings.VerticalAlignment = TextAlignmentType.Center;

            // Applicera standardstilinställningarna på det första bladet
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells.ApplyStyle(workbook.CreateStyle(), new StyleFlag() { All = true });

            // Spara arbetsboken
            workbook.Save("DefaultStyleSettingsExample.xlsx");
            workbook.Save("DefaultStyleSettingsExample.pdf");

            return;
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


