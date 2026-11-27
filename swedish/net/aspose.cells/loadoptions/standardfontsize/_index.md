---
title: "LoadOptions.StandardFontSize"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions-egenskap. Anger standardteckensnittets storlek"
type: docs
url: /sv/net/aspose.cells/loadoptions/standardfontsize/
---
## LoadOptions.StandardFontSize property

Anger standardteckensnittets standardstorlek.

```csharp
[Obsolete("Use DefaultStyleSettings.FontSize property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double StandardFontSize { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället DefaultStyleSettings. Denna egenskap kommer att tas bort 12 månader senare sedan mars 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyStandardFontSizeDemo
    {
        public static void Run()
        {
            // Skapa HTML‑laddningsalternativ och ange StandardFontSize
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            loadOptions.StandardFont = "Calibri";
            loadOptions.StandardFontSize = 11;

            // Läs in arbetsboken med alternativen
            Workbook workbook = new Workbook(new MemoryStream(), loadOptions);
            
            // Åtkomst till första arbetsbladet och cellerna
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // Ange lite exempeltext och verifiera teckensnittsegenskaper
            cells["A1"].PutValue("Sample Text");
            Style style = cells["A1"].GetStyle();
            
            Console.WriteLine("Font Name: " + style.Font.Name);
            Console.WriteLine("Font Size: " + style.Font.Size);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


