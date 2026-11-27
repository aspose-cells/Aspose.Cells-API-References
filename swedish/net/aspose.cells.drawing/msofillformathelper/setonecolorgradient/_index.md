---
title: "MsoFillFormatHelper.SetOneColorGradient"
second_title: "Aspose.Cells för .NET API‑referens"
description: "MsoFillFormatHelper-metod. Ställer in den angivna fyllningen till en enfärgsgradient"
type: docs
url: /sv/net/aspose.cells.drawing/msofillformathelper/setonecolorgradient/
---
## MsoFillFormatHelper.SetOneColorGradient method

Ställer in den angivna fyllningen till en enfärgsgradient.

```csharp
public void SetOneColorGradient(Color color, double degree, GradientStyleType style, int variant)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| färg | Färg | En gradientfärg. |
| grad | Double | Gradientens grad. Kan vara ett värde från 0,0 (mörk) till 1,0 (ljus). |
| style | GradientStyleType | Gradientskuggningsstil. |
| variant | Int32 | Gradientvarianten. Kan vara ett värde från 1 till 4, motsvarande en av de fyra varianterna på fliken Gradient i dialogrutan Fylleffekter. Om stil är GradientStyle.FromCenter, kan Variant‑argumentet endast vara 1 eller 2. |

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;
    using System.Drawing;

    public class MsoFillFormatHelperMethodSetOneColorGradientWithColorDoubleGradientStyleTyInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och hämta det första kalkylbladet
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Placera en enkel etikett i bladet för kontext
            worksheet.Cells["A1"].Value = "Gradient Fill Demo";

            try
            {
                // Skapa en instans av MsoFillFormatHelper med reflektion (ingen publik ctor)
                MsoFillFormatHelper fillHelper = (MsoFillFormatHelper)Activator.CreateInstance(
                    typeof(MsoFillFormatHelper), nonPublic: true);

                // Parametrar för gradienten
                Color gradientColor = Color.FromArgb(255, 0, 120, 215); // a shade of blue
                double degree = 45.0;                                 // gradient angle in degrees
                GradientStyleType style = GradientStyleType.Horizontal; // horizontal gradient
                int variant = 0;                                      // variant (0 = default)

                // Applicera den enfärgade gradienten
                fillHelper.SetOneColorGradient(gradientColor, degree, style, variant);

                // Valfritt: visa att egenskaperna kan läsas efter anropet
                Console.WriteLine($"ForeColor after gradient: {fillHelper.ForeColor}");
                Console.WriteLine($"ForeColorTransparency after gradient: {fillHelper.ForeColorTransparency}");

                // Spara arbetsboken (ingen visuell förändring kommer att ses eftersom hjälpen inte är kopplad till en form)
                workbook.Save("SetOneColorGradientDemo.xlsx");

                Console.WriteLine("SetOneColorGradient method called successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error calling SetOneColorGradient: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [GradientStyleType](../../gradientstyletype/)
* class [MsoFillFormatHelper](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


