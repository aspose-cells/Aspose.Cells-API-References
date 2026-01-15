---
title: IndividualFontConfigs.GetFontSubstitutes
second_title: Aspose.Cells for .NET API Reference
description: IndividualFontConfigs method. Returns an array containing font substitute names to be used if original font is not presented
type: docs
url: /net/aspose.cells/individualfontconfigs/getfontsubstitutes/
---
## IndividualFontConfigs.GetFontSubstitutes method

Returns an array containing font substitute names to be used if original font is not presented.

```csharp
public string[] GetFontSubstitutes(string originalFontName)
```

| Parameter | Type | Description |
| --- | --- | --- |
| originalFontName | String | originalFontName |

### Return Value

An array containing font substitute names to be used if original font is not presented.

### Examples

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class IndividualFontConfigsMethodGetFontSubstitutesWithStringDemo
    {
        public static void Run()
        {
            // Create individual font configurations
            IndividualFontConfigs fontConfigs = new IndividualFontConfigs();

            // Set font substitutes for "Arial"
            fontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman", "Calibri" });

            try
            {
                // Get font substitutes for "Arial"
                string[] substitutes = fontConfigs.GetFontSubstitutes("Arial");

                Console.WriteLine("Font substitutes for Arial:");
                foreach (string font in substitutes)
                {
                    Console.WriteLine(font);
                }

                // Create a workbook to demonstrate the effect
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Set style with original font
                Style style = workbook.CreateStyle();
                style.Font.Name = "Arial";
                worksheet.Cells["A1"].SetStyle(style);
                worksheet.Cells["A1"].Value = "This text uses Arial font which may be substituted";

                // Save the workbook
                workbook.Save("FontSubstitutesDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetFontSubstitutes method: {ex.Message}");
            }
        }
    }
}
```

### See Also

* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


