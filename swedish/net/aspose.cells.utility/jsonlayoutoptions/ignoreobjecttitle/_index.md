---
title: "JsonLayoutOptions.IgnoreObjectTitle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonLayoutOptions-egenskap. Anger om titeln ska ignoreras när objektet är en egenskap till ett annat objekt"
type: docs
url: /sv/net/aspose.cells.utility/jsonlayoutoptions/ignoreobjecttitle/
---
## JsonLayoutOptions.IgnoreObjectTitle property

Anger om titeln ska ignoreras när objektet är en egenskap till ett annat objekt.

```csharp
[Obsolete("Use JsonLayoutOptions.IgnoreTitle property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IgnoreObjectTitle { get; set; }
```

### Anmärkningar

OBS: Den här egenskapen är nu föråldrad. Använd istället JsonLayoutOptions.IgnoreTitle-egenskapen. Den här egenskapen kommer att tas bort 6 månader senare sedan februari 2023. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Utility;
    using System;

    public class JsonLayoutOptionsPropertyIgnoreObjectTitleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempel på JSON-data med objekttitlar
            string json = @"{
                ""Employees"": {
                    ""Employee"": [
                        { ""Name"": ""John"", ""Age"": 30 },
                        { ""Name"": ""Jane"", ""Age"": 25 }
                    ]
                }
            }";

            // Skapa JsonLayoutOptions
            JsonLayoutOptions options = new JsonLayoutOptions();
            
            // Visa aktuellt IgnoreObjectTitle-värde
            Console.WriteLine("Current IgnoreObjectTitle value: " + options.IgnoreObjectTitle);

            // Ställ in för att ignorera objekttitlar
            options.IgnoreObjectTitle = true;
            Console.WriteLine("Set IgnoreObjectTitle to: " + options.IgnoreObjectTitle);

            // Importera JSON med IgnoreObjectTitle = true
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);

            // Spara med ignorerade titlar
            workbook.Save("IgnoreObjectTitle_True.xlsx");

            // Återställ kalkylbladet
            worksheet.Cells.Clear();

            // Ställ in för att inkludera objekttitlar
            options.IgnoreObjectTitle = false;
            Console.WriteLine("Set IgnoreObjectTitle to: " + options.IgnoreObjectTitle);

            // Importera JSON med IgnoreObjectTitle = false
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);

            // Spara med inkluderade titlar
            workbook.Save("IgnoreObjectTitle_False.xlsx");
        }
    }
}
```

### Se även

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


