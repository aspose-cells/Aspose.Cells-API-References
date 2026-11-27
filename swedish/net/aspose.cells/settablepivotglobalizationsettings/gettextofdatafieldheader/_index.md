---
title: "SettablePivotGlobalizationSettings.GetTextOfDataFieldHeader"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettablePivotGlobalizationSettings-metoden. Hämtar texten för fältets rubrik i värdeområdet i pivottabellen"
type: docs
url: /sv/net/aspose.cells/settablepivotglobalizationsettings/gettextofdatafieldheader/
---
## SettablePivotGlobalizationSettings.GetTextOfDataFieldHeader method

Hämtar texten för rubriken på värdeområdesfältet i pivottabellen.

```csharp
public override string GetTextOfDataFieldHeader()
```

### Returvärde

Texten för datafältets rubriknamn

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfDataFieldHeaderDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till lite exempeldata för sammanhang
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Skapa en instans av SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Hämta standardtexten för datafältets rubrik
                string dataFieldHeaderText = settings.GetTextOfDataFieldHeader();
                Console.WriteLine($"Default data field header text: {dataFieldHeaderText}");

                // Ange en anpassad text för datafältets rubrik
                settings.SetTextOfDataFieldHeader("Custom Data Header");
                dataFieldHeaderText = settings.GetTextOfDataFieldHeader();
                Console.WriteLine($"Updated data field header text: {dataFieldHeaderText}");

                // Spara arbetsboken
                workbook.Save("GetTextOfDataFieldHeaderDemo.xlsx");
                Console.WriteLine("GetTextOfDataFieldHeader method called successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfDataFieldHeader: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


