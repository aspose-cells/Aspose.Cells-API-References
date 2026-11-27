---
title: "AutoNumberedBulletValue.AutonumberScheme"
second_title: "Aspose.Cells för .NET API‑referens"
description: "AutoNumberedBulletValue‑egenskap. Representerar schemat för automatiskt nummer"
type: docs
url: /sv/net/aspose.cells.drawing.texts/autonumberedbulletvalue/autonumberscheme/
---
## AutoNumberedBulletValue.AutonumberScheme property

Representerar schemat för automatiskt nummer.

```csharp
public TextAutonumberScheme AutonumberScheme { get; set; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.Texts;
    using System;

    public class AutoNumberedBulletValuePropertyAutonumberSchemeDemo
    {
        public static void Run()
        {
            try
            {
                // Skapa en ny AutoNumberedBulletValue‑instans
                AutoNumberedBulletValue bullet = new AutoNumberedBulletValue();

                // Visa initialt AutonumberScheme‑värde
                Console.WriteLine($"Default AutonumberScheme: {bullet.AutonumberScheme}");

                // Ange ett nytt AutonumberScheme‑värde
                bullet.AutonumberScheme = TextAutonumberScheme.RomanUcPeriod;
                Console.WriteLine($"Modified AutonumberScheme: {bullet.AutonumberScheme}");

                // Skapa en arbetsbok för att demonstrera bullet i sammanhang
                Workbook workbook = new Workbook();
                Worksheet worksheet = workbook.Worksheets[0];

                // Skapa en form med text som kommer att använda bullet‑stilen
                TextBox shape = worksheet.Shapes.AddTextBox(1, 0, 1, 100, 300, 100);
                shape.TextBody.Text = "Sample text with bullet formatting";


                // Obs: Faktisk tillämpning av bullet‑stilen på text skulle kräva ytterligare API‑anrop
                // Visas inte i reflektionen. Vi sparar bara arbetsboken som demonstration.
                workbook.Save("AutonumberSchemeDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Se även

* enum [TextAutonumberScheme](../../textautonumberscheme/)
* class [AutoNumberedBulletValue](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


