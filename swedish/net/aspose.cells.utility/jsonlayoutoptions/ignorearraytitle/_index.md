---
title: "JsonLayoutOptions.IgnoreArrayTitle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "JsonLayoutOptions‑egenskap. Anger om titeln ska ignoreras när en array är en egenskap i ett objekt"
type: docs
url: /sv/net/aspose.cells.utility/jsonlayoutoptions/ignorearraytitle/
---
## JsonLayoutOptions.IgnoreArrayTitle property

Anger om titeln ska ignoreras när en array är en egenskap i ett objekt.

```csharp
[Obsolete("Use JsonLayoutOptions.IgnoreTitle property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool IgnoreArrayTitle { get; set; }
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

    public class JsonLayoutOptionsPropertyIgnoreArrayTitleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Exempel på JSON-data med arraytitlar
            string json = @"{
                ""Employees"": [
                    { ""Name"": ""John"", ""Age"": 30 },
                    { ""Name"": ""Jane"", ""Age"": 25 }
                ]
            }";

            // Skapa JsonLayoutOptions
            JsonLayoutOptions options = new JsonLayoutOptions();
            
            // Visa aktuellt IgnoreArrayTitle-värde
            Console.WriteLine("Current IgnoreArrayTitle value: " + options.IgnoreArrayTitle);

            // Första importen med IgnoreArrayTitle = false (standard)
            options.IgnoreArrayTitle = false;
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);
            Console.WriteLine("Data imported with IgnoreArrayTitle=false. Check cell A1 for 'Employees' title.");

            // Rensa arbetsbladet för andra importen
            worksheet.Cells.Clear();

            // Andra importen med IgnoreArrayTitle = true
            options.IgnoreArrayTitle = true;
            JsonUtility.ImportData(json, worksheet.Cells, 0, 0, options);
            Console.WriteLine("Data imported with IgnoreArrayTitle=true. Check cell A1 for direct array values.");

            // Spara arbetsboken
            workbook.Save("JsonLayoutOptionsIgnoreArrayTitleDemo.xlsx");
        }
    }
}
```

### Se även

* class [JsonLayoutOptions](../)
* namespace [Aspose.Cells.Utility](../../../aspose.cells.utility/)
* assembly [Aspose.Cells](../../../)


