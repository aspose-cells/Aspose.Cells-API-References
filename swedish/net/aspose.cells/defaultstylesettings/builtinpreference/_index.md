---
title: "DefaultStyleSettings.BuiltInPreference"
second_title: "Aspose.Cells för .NET API‑referens"
description: "DefaultStyleSettings-egenskap. Anger om egenskapen för talformat är föredragen när stilen definierar både inbyggt tal och anpassat mönster. Standardvärdet är falskt, vilket betyder att som standard det anpassade mönstret kommer att användas för att formatera värden så länge det inte är tomt för en stil."
type: docs
url: /sv/net/aspose.cells/defaultstylesettings/builtinpreference/
---
## DefaultStyleSettings.BuiltInPreference property

Indikerar om egenskapen för talformat är att föredra när stilen definierar både inbyggt talformat och anpassat mönster. Standardvärdet är false, vilket betyder att standardmässigt kommer det anpassade mönstret att användas för att formatera värden så länge det inte är tomt för en stil.

```csharp
public bool BuiltInPreference { get; set; }
```

### Anmärkningar

När en arbetsbok laddas från en befintlig mallfil kan både inbyggt tal och anpassat mönster vara definierade för en stil. Denna egenskap bestämmer om vi ska använda det inbyggda talet eller det anpassade mönstret när värden formateras med stilen.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyBuiltInPreferenceDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Åtkomst till standardstilinställningar
            DefaultStyleSettings defaultStyleSettings = workbook.Settings.DefaultStyleSettings;

            // Demonstrera egenskapen BuiltInPreference
            defaultStyleSettings.BuiltInPreference = false;
            defaultStyleSettings.FontName = "Arial";
            defaultStyleSettings.FontSize = 12;

            // Tillämpa på kalkylblad
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Text");
            
            // Spara arbetsboken
            workbook.Save("BuiltInPreferenceDemo.xlsx");
        }
    }
}
```

### Se även

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


