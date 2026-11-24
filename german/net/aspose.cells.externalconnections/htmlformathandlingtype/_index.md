---
title: "Enum HtmlFormatHandlingType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.ExternalConnections.HtmlFormatHandlingType Enum. Gibt an, wie die Formatierung aus der HTML-Quelle zu behandeln ist"
type: docs
url: /de/net/aspose.cells.externalconnections/htmlformathandlingtype/
---
## HtmlFormatHandlingType enumeration

Gibt an, wie die Formatierung aus der HTML-Quelle zu behandeln ist

```csharp
public enum HtmlFormatHandlingType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| All | `0` | Übertrage alle HTML-Formatierungen zusammen mit den Daten in das Arbeitsblatt. |
| None | `1` | Bringe Daten als unformatierten Text ein (Festlegen der Datentypen erfolgt weiterhin). |
| Rtf | `2` | Übersetze HTML-Formatierung in Rich-Text-Formatierung für die in das Arbeitsblatt eingefügten Daten. |

### Beispiele

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
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Demonstriere alle Enum-Werte von HtmlFormatHandlingType
                HtmlFormatHandlingType allFormatting = HtmlFormatHandlingType.All;
                HtmlFormatHandlingType noFormatting = HtmlFormatHandlingType.None;
                HtmlFormatHandlingType rtfFormatting = HtmlFormatHandlingType.Rtf;

                // Die Enum-Werte anzeigen
                Console.WriteLine("HtmlFormatHandlingType.All: " + allFormatting);
                Console.WriteLine("HtmlFormatHandlingType.None: " + noFormatting);
                Console.WriteLine("HtmlFormatHandlingType.Rtf: " + rtfFormatting);

                // Simuliere die Verwendung dieser Werte in einem Szenario
                worksheet.Cells["A1"].PutValue("Format Handling Types:");
                worksheet.Cells["A2"].PutValue("All Formatting");
                worksheet.Cells["A3"].PutValue("No Formatting");
                worksheet.Cells["A4"].PutValue("RTF Formatting");

                // Speichere die Arbeitsmappe
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

### Siehe auch

* namespace [Aspose.Cells.ExternalConnections](../../aspose.cells.externalconnections/)
* assembly [Aspose.Cells](../../)


