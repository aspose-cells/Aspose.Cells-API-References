---
title: "LoadOptions.StandardFont"
second_title: "Aspose.Cells för .NET API‑referens"
description: "LoadOptions egenskap. Anger standardteckensnittets namn"
type: docs
url: /sv/net/aspose.cells/loadoptions/standardfont/
---
## LoadOptions.StandardFont property

Anger standardteckensnittets namn

```csharp
[Obsolete("Use DefaultStyleSettings.FontName property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StandardFont { get; set; }
```

### Anmärkningar

OBS: Denna medlem är nu föråldrad. Använd istället DefaultStyleSettings. Denna egenskap kommer att tas bort 12 månader senare sedan mars 2022. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyStandardFontDemo
    {
        public static void Run()
        {
            // Skapa en exempel‑Excel‑fil i minnet
            MemoryStream ms = new MemoryStream();
            using (Workbook workbook = new Workbook())
            {
                workbook.Worksheets[0].Cells["A1"].PutValue("Standard Font Test");
                workbook.Save(ms, SaveFormat.Xlsx);
            }
            ms.Position = 0;

            // Ställ in laddningsalternativ med StandardFont
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.StandardFont = "SimSun";
            
            // Läs in arbetsbok med det angivna teckensnittet
            Workbook workbookWithFont = new Workbook(ms, loadOptions);
            
            // Visa att teckensnittet är inställt genom att kontrollera standardstilen
            Console.WriteLine("Default font after loading: " + 
                workbookWithFont.DefaultStyle.Font.Name);
        }
    }
}
```

### Se även

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


