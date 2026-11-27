---
title: "SettablePivotGlobalizationSettings.GetTextOfRowLabels"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SettablePivotGlobalizationSettings‑metod. Hämtar texten för etiketten Row Labels i pivottabellen"
type: docs
url: /sv/net/aspose.cells/settablepivotglobalizationsettings/gettextofrowlabels/
---
## SettablePivotGlobalizationSettings.GetTextOfRowLabels method

Hämtar texten för etiketten "Row Labels" i PivotTable.

```csharp
public override string GetTextOfRowLabels()
```

### Returvärde

Texten för radetiketter

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SettablePivotGlobalizationSettingsMethodGetTextOfRowLabelsDemo
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
                // Ange anpassad text för radetiketter
                settings.SetTextOfRowLabels("Custom Row Labels");

                // Hämta texten för radetiketter
                string rowLabelsText = settings.GetTextOfRowLabels();

                Console.WriteLine($"Text of Row Labels: {rowLabelsText}");

                // Spara arbetsboken
                workbook.Save("GetTextOfRowLabelsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling GetTextOfRowLabels: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [SettablePivotGlobalizationSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


