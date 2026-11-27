---
title: "OoxmlSaveOptions.AsFlatOpc"
second_title: "Aspose.Cells för .NET API‑referens"
description: "OoxmlSaveOptions-egenskap. Anger om sparas som en flat opc-fil som kan genereras av Open XML SDK"
type: docs
url: /sv/net/aspose.cells/ooxmlsaveoptions/asflatopc/
---
## OoxmlSaveOptions.AsFlatOpc property

Anger om sparas som en platt OPC‑fil som kan genereras av Open XML SDK.

```csharp
public bool AsFlatOpc { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlSaveOptionsPropertyAsFlatOpcDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();

            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till data för att göra exemplet meningsfullt
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["B1"].PutValue("Flat OPC Demo");

            try
            {
                // Skapa en OoxmlSaveOptions-instans
                OoxmlSaveOptions saveOptions = new OoxmlSaveOptions();

                // Visa standardvärdet för AsFlatOpc-egenskapen
                Console.WriteLine("Default AsFlatOpc value: " + saveOptions.AsFlatOpc);

                // Ställ in AsFlatOpc till true
                saveOptions.AsFlatOpc = true;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions.AsFlatOpc);

                // Spara arbetsboken med AsFlatOpc aktiverat
                workbook.Save("AsFlatOpc_Enabled.xlsx", saveOptions);

                // Skapa ett annat sparalternativ med AsFlatOpc inaktiverat
                OoxmlSaveOptions saveOptions2 = new OoxmlSaveOptions();
                saveOptions2.AsFlatOpc = false;
                Console.WriteLine("AsFlatOpc set to: " + saveOptions2.AsFlatOpc);

                // Spara arbetsboken med AsFlatOpc inaktiverat
                workbook.Save("AsFlatOpc_Disabled.xlsx", saveOptions2);

                Console.WriteLine("AsFlatOpc property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


