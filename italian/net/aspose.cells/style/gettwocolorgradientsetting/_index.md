---
title: "Style.GetTwoColorGradientSetting"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo Style. Ottieni l'impostazione del gradiente a due colori"
type: docs
url: /it/net/aspose.cells/style/gettwocolorgradientsetting/
---
## Style.GetTwoColorGradientSetting method

Ottieni l'impostazione del gradiente a due colori.

```csharp
public TwoColorGradient GetTwoColorGradientSetting()
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea uno stile e imposta un gradiente a due colori
            Style style = workbook.CreateStyle();
            style.SetTwoColorGradient(Color.Red, Color.Blue, GradientStyleType.Horizontal, 1);
            style.IsGradient = true;

            // Applica lo stile a una cella
            Cell cell = worksheet.Cells["A1"];
            cell.PutValue("Two Color Gradient Demo");
            cell.SetStyle(style);

            try
            {
                // Chiama il metodo GetTwoColorGradientSetting
                TwoColorGradient gradientSetting = style.GetTwoColorGradientSetting();

                // Visualizza le impostazioni del gradiente
                Console.WriteLine("Color1: " + gradientSetting.Color1);
                Console.WriteLine("Color2: " + gradientSetting.Color2);
                Console.WriteLine("GradientStyleType: " + gradientSetting.GradientStyleType);
                Console.WriteLine("Variant: " + gradientSetting.Variant);

                // Modifica le impostazioni del gradiente
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

            // Salva il risultato
            workbook.Save("MethodGetTwoColorGradientSettingDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [TwoColorGradient](../../twocolorgradient/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


