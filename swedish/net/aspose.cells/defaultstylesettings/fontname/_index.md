---
title: "DefaultStyleSettings.FontName"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Egenskapen DefaultStyleSettings. Hämtar/Anger standardteckensnittets namn för arbetsboken"
type: docs
url: /sv/net/aspose.cells/defaultstylesettings/fontname/
---
## DefaultStyleSettings.FontName property

Hämtar/Anger standardtypsnittets namn för arbetsboken

```csharp
public string FontName { get; set; }
```

### Exempel

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyFontNameDemo
    {
        public static void Run()
        {
            // Skapa laddningsalternativ och ange teckensnittets namn
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
            loadOptions.DefaultStyleSettings.FontName = "SimSun";

            // Skapa en ny arbetsbok med laddningsalternativen
            Workbook workbook = new Workbook();
            workbook.DefaultStyle.Font.Name = loadOptions.DefaultStyleSettings.FontName;

            // Få åtkomst till standardstilen och verifiera teckensnittets namn
            Style defaultStyle = workbook.DefaultStyle;
            Console.WriteLine("Default Font Name: " + defaultStyle.Font.Name);

            // Skapa ett kalkylblad och ange cellvärde
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Font Name Test");

            // Spara arbetsboken
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, SaveFormat.Xlsx);
                Console.WriteLine("Workbook saved with default font: SimSun");
            }
        }
    }
}
```

### Se även

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


