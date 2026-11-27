---
title: "Style.GetTwoColorGradientSetting"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Style-metod. Hämta tvåfärgsgradientinställningen"
type: docs
url: /sv/net/aspose.cells/style/gettwocolorgradientsetting/
---
## Style.GetTwoColorGradientSetting method

Hämta den tvåfärgade gradientinställningen.

```csharp
public TwoColorGradient GetTwoColorGradientSetting()
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class StyleMethodGetTwoColorGradientSettingDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en stil och ange tvåfärgsgradient
            Style style = workbook.CreateStyle();
            style.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 1);
            style.IsGradient = true;

            // Tillämpa stilen på en cell
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Two Color Gradient Demo");
            cell.SetStyle(style);

            try
            {
                // Anropa metoden GetTwoColorGradientSetting
                TwoColorGradient gradientSetting = style.GetTwoColorGradientSetting();

                // Visa gradientinställningarna
                Console.WriteLine("Color1: " + gradientSetting.Color1);
                Console.WriteLine("Color2: " + gradientSetting.Color2);
                Console.WriteLine("GradientStyleType: " + gradientSetting.GradientStyleType);
                Console.WriteLine("Variant: " + gradientSetting.Variant);

                // Modifiera gradientinställningarna
                gradientSetting.Color1 = Color.Green;
                gradientSetting.GradientStyleType = GradientStyleType.Vertical;
                style.SetTwoColorGradient(gradientSetting.Color1, gradientSetting.Color2, 
                                        gradientSetting.GradientStyleType, gradientSetting.Variant);

                Console.WriteLine("Gradient settings modified successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetTwoColorGradientSetting method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("MethodGetTwoColorGradientSettingDemo.xlsx");
        }
    }
}
```

### Se även

* class [TwoColorGradient](../../twocolorgradient/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


