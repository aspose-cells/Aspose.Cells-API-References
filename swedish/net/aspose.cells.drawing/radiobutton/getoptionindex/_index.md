---
title: "RadioButton.GetOptionIndex"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RadioButton‑metod. Hämtar alternativindex, enbaserat, för alla radioknappar i GroupBox som innehåller denna radioknapp"
type: docs
url: /sv/net/aspose.cells.drawing/radiobutton/getoptionindex/
---
## RadioButton.GetOptionIndex method

Hämtar alternativindexet (enbaserat) i alla radioknappar i GroupBox som innehåller den här radioknappen.

```csharp
public int GetOptionIndex()
```

### Anmärkningar

Om denna radioknapp inte är i GroupBox returneras alternativindex för alla radioknappar som inte finns i någon GroupBox

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class RadioButtonMethodGetOptionIndexDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en GroupBox för att innehålla radioknappar
            GroupBox groupBox = worksheet.Shapes.AddGroupBox(1, 0, 100, 200, 100, 200);

            // Lägg till tre radioknappar i GroupBox
            RadioButton radioButton1 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 20, 100, 20, 100);
            RadioButton radioButton2 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 50, 100, 20, 100);
            RadioButton radioButton3 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 80, 100, 20, 100);

            // Ställ in radioknapparna så att de blir en del av GroupBox
            radioButton1.Placement = PlacementType.FreeFloating;
            radioButton2.Placement = PlacementType.FreeFloating;
            radioButton3.Placement = PlacementType.FreeFloating;

            try
            {
                // Hämta alternativindex för varje radioknapp
                int index1 = radioButton1.GetOptionIndex();
                int index2 = radioButton2.GetOptionIndex();
                int index3 = radioButton3.GetOptionIndex();

                Console.WriteLine($"RadioButton1 Option Index: {index1}");
                Console.WriteLine($"RadioButton2 Option Index: {index2}");
                Console.WriteLine($"RadioButton3 Option Index: {index3}");

                // Markera den första radioknappen för att demonstrera urval
                radioButton1.IsChecked = true;
                Console.WriteLine("RadioButton1 is checked");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing GetOptionIndex method: {ex.Message}");
            }

            // Spara resultatet
            workbook.Save("RadioButtonMethodGetOptionIndexDemo.xlsx");
        }
    }
}
```

### Se även

* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


