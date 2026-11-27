---
title: "Enum HtmlFormatHandlingType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.ExternalConnections.HtmlFormatHandlingType enum. Anger hur formatering från HTML-källan ska hanteras"
type: docs
url: /sv/net/aspose.cells.externalconnections/htmlformathandlingtype/
---
## HtmlFormatHandlingType enumeration

Anger hur formatering från HTML-källan ska hanteras

```csharp
public enum HtmlFormatHandlingType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| All | `0` | Överför all HTML-formatering till arbetsbladet tillsammans med data. |
| None | `1` | Importera data som oformaterad text (inställning av datatyper sker fortfarande). |
| Rtf | `2` | Översätt HTML-formatering till riktextformatering på data som importeras till arbetsbladet. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.ExternalConnections;
    using System;

    public class ExternalConnectionsClassHtmlFormatHandlingTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Demonstrera alla enum‑värden för HtmlFormatHandlingType
                HtmlFormatHandlingType allFormatting = HtmlFormatHandlingType.All;
                HtmlFormatHandlingType noFormatting = HtmlFormatHandlingType.None;
                HtmlFormatHandlingType rtfFormatting = HtmlFormatHandlingType.Rtf;

                // Visa enum‑värden
                Console.WriteLine("HtmlFormatHandlingType.All: " + allFormatting);
                Console.WriteLine("HtmlFormatHandlingType.None: " + noFormatting);
                Console.WriteLine("HtmlFormatHandlingType.Rtf: " + rtfFormatting);

                // Simulera användning av dessa värden i ett scenario
                worksheet.Cells["A1"].PutValue("Format Handling Types:");
                worksheet.Cells["A2"].PutValue("All Formatting");
                worksheet.Cells["A3"].PutValue("No Formatting");
                worksheet.Cells["A4"].PutValue("RTF Formatting");

                // Spara arbetsboken
                workbook.Save("HtmlFormatHandlingTypeDemo.xlsx");
                Console.WriteLine("Demo completed successfully. File saved.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in HtmlFormatHandlingType demo: {ex.Message}");
            }
        }
    }
}
```

### Se även

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


