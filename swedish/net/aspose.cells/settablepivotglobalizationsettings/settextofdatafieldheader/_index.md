---
title: "SettablePivotGlobalizationSettings.SetTextOfDataFieldHeader"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettablePivotGlobalizationSettings‑metod. Anger texten för rubriken i värdeområdet i pivottabellen"
type: docs
url: /sv/net/aspose.cells/settablepivotglobalizationsettings/settextofdatafieldheader/
---
## SettablePivotGlobalizationSettings.SetTextOfDataFieldHeader method

Ställer in texten för rubriken för värdeområdesfältet i PivotTable.

```csharp
public void SetTextOfDataFieldHeader(string text)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| text | String | Texten för datafältets rubriknamn |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodSetTextOfDataFieldHeaderWithStringDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);

            // Skapa en instans av SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Ange anpassad text för datafältets rubrik
                settings.SetTextOfDataFieldHeader("Custom Data Header");

                // Verifiera ändringen genom att hämta den aktuella texten
                string currentHeaderText = settings.GetTextOfDataFieldHeader();
                Console.WriteLine($"Data field header text: {currentHeaderText}");

                // Spara arbetsboken för att demonstrera en lyckad körning
                workbook.Save("SetTextOfDataFieldHeaderDemo.xlsx");
                Console.WriteLine("SetTextOfDataFieldHeader method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetTextOfDataFieldHeader: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


