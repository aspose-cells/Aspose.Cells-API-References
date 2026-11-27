---
title: "LoadOptions.DefaultStyleSettings"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions‑egenskap. Hämtar standardstilsinställningarna för att initiera stilar i arbetsboken"
type: docs
url: /sv/net/aspose.cells/loadoptions/defaultstylesettings/
---
## LoadOptions.DefaultStyleSettings property

Hämtar standardinställningarna för stil vid initiering av arbetsbokens stilar.

```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyDefaultStyleSettingsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Ange laddningsalternativ med standardstilsinställningar
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
            loadOptions.DefaultStyleSettings.VerticalAlignment = TextAlignmentType.Bottom;
            
            // Skapa ett kalkylblad och hämta celler
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Ange värden för att demonstrera standardstilen
            cells["A1"].PutValue("Default Style Applied");
            cells["A2"].PutValue("Should have bottom alignment");
            
            // Skapa en cell med anpassad stil (för att kontrastera med standard)
            Cell customCell = cells["B1"];
            customCell.PutValue("Custom Style");
            Style customStyle = customCell.GetStyle();
            customStyle.VerticalAlignment = TextAlignmentType.Center;
            customCell.SetStyle(customStyle);
            
            // Spara arbetsboken
            workbook.Save("DefaultStyleSettingsDemo.xlsx");
            
            // Verifiera stilarna
            Console.WriteLine("A1 Vertical Alignment: " + cells["A1"].GetStyle().VerticalAlignment);
            Console.WriteLine("B1 Vertical Alignment: " + cells["B1"].GetStyle().VerticalAlignment);
        }
    }
}
```

### Se även

* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


