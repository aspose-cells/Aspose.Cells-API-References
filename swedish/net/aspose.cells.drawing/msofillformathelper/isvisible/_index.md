---
title: "MsoFillFormatHelper.IsVisible"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFillFormatHelper-egenskap. Anger om det finns fyllning"
type: docs
url: /sv/net/aspose.cells.drawing/msofillformathelper/isvisible/
---
## MsoFillFormatHelper.IsVisible property

Indikerar om det finns fyllning.

```csharp
public bool IsVisible { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en etikett för att göra exemplet meningsfullt
            worksheet.Cells["A1"].Value = "IsVisible Property Demo";

            try
            {
                // Skapa en instans av MsoFillFormatHelper med hjälp av reflektion (ingen publik konstruktor)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Visa standardvärdet för IsVisible
                Console.WriteLine($"Default IsVisible: {fillHelper.IsVisible}");

                // Ställ in IsVisible till true
                fillHelper.IsVisible = true;
                Console.WriteLine($"After setting to true: {fillHelper.IsVisible}");

                // Ställ in IsVisible till false
                fillHelper.IsVisible = false;
                Console.WriteLine($"After setting to false: {fillHelper.IsVisible}");

                // Läs det aktuella IsVisible-värdet
                bool isVisible = fillHelper.IsVisible;
                Console.WriteLine($"Current IsVisible value: {isVisible}");

                // Spara arbetsboken för att demonstrera en lyckad körning
                workbook.Save("IsVisibleDemo.xlsx");

                Console.WriteLine("IsVisible property demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error during IsVisible demo: {ex.Message}");
            }
        }
    }
}
```

### Se även

* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


