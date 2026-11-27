---
title: "SettablePivotGlobalizationSettings.GetTextOfColumnLabels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettablePivotGlobalizationSettings-metod. Hämtar texten för etiketten Kolumnrubriker i pivottabellen"
type: docs
url: /sv/net/aspose.cells/settablepivotglobalizationsettings/gettextofcolumnlabels/
---
## SettablePivotGlobalizationSettings.GetTextOfColumnLabels method

Hämtar texten för etiketten "Column Labels" i pivottabellen.

```csharp
public override string GetTextOfColumnLabels()
```

### Returvärde

Texten för kolumnrubriker

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfColumnLabelsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för sammanhang
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);

            // Skapa en instans av SettablePivotGlobalizationSettings
            SettablePivotGlobalizationSettings settings = new SettablePivotGlobalizationSettings();

            try
            {
                // Hämta standardtexten för kolumnetiketter
                string columnLabelsText = settings.GetTextOfColumnLabels();
                Console.WriteLine($"Default text of Column Labels: {columnLabelsText}");

                // Ange anpassad text för kolumnetiketter
                settings.SetTextOfColumnLabels("Custom Column Headers");

                // Hämta den uppdaterade texten för kolumnetiketter
                string updatedColumnLabelsText = settings.GetTextOfColumnLabels();
                Console.WriteLine($"Updated text of Column Labels: {updatedColumnLabelsText}");

                // Spara arbetsboken
                workbook.Save("GetTextOfColumnLabelsDemo.xlsx");
                Console.WriteLine("GetTextOfColumnLabels method executed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfColumnLabels: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


