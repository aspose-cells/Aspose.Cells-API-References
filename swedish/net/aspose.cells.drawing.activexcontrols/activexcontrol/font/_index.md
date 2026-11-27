---
title: "ActiveXControl.Font"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ActiveXControl egenskap. Representerar kontrollens teckensnitt"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/activexcontrol/font/
---
## ActiveXControl.Font property

Representerar teckensnittet för kontrollen.

```csharp
public Font Font { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlPropertyFontDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Lägg till en ActiveX-kontroll (Label) i kalkylbladet
                Shape shape = worksheet.Shapes.AddActiveXControl(
                    ControlType.Label,
                    1, 1, 200, 50,
                    0, 0);

                // Hämta instansen av ActiveX-kontrollen
                LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

                // Ställ in några grundläggande egenskaper
                label.Caption = "Sample Label";

                // Åtkomst till Font-egenskapen (skrivskyddad)
                Font controlFont = label.Font;

                // Visa teckensnittsegenskaper
                Console.WriteLine("Font Name: " + controlFont.Name);
                Console.WriteLine("Font Size: " + controlFont.Size);
                Console.WriteLine("Is Bold: " + controlFont.IsBold);
                Console.WriteLine("Is Italic: " + controlFont.IsItalic);
                Console.WriteLine("Color: " + controlFont.Color);
                Console.WriteLine("Underline Type: " + controlFont.Underline);

                // Spara arbetsboken
                workbook.Save("FontDemo.xlsx");
                Console.WriteLine("Font properties demonstrated successfully.");
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

* class [Font](../../../aspose.cells/font/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


