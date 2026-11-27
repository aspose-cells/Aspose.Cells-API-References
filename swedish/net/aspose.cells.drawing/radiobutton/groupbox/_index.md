---
title: "RadioButton.GroupBox"
second_title: "Aspose.Cells för .NET API‑referens"
description: "RadioButton-egenskap. Hämtar GroupBox som innehåller denna RadioButton"
type: docs
url: /sv/net/aspose.cells.drawing/radiobutton/groupbox/
---
## RadioButton.GroupBox property

Hämtar GroupBox som innehåller den här RadioButton.

```csharp
public GroupBox GroupBox { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class RadioButtonPropertyGroupBoxDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en GroupBox för att innehålla radioknappar
            GroupBox groupBox = worksheet.Shapes.AddGroupBox(1, 0, 100, 200, 100, 200);
            groupBox.Name = "OptionsGroup";
            groupBox.Shadow = true;

            // Lägg till radioknappar i arbetsbladet (ännu inte i GroupBox)
            RadioButton radioButton1 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 20, 100, 20, 100);
            RadioButton radioButton2 = (RadioButton)worksheet.Shapes.AddRadioButton(3, 0, 50, 100, 20, 100);

            // Visa initiala GroupBox-egenskapsvärden (bör vara null)
            Console.WriteLine("RadioButton1 GroupBox before grouping: " + (radioButton1.GroupBox == null ? "null" : radioButton1.GroupBox.Name));
            Console.WriteLine("RadioButton2 GroupBox before grouping: " + (radioButton2.GroupBox == null ? "null" : radioButton2.GroupBox.Name));

            // Lägg till radioknappar i GroupBox genom att ange placering
            radioButton1.Placement = PlacementType.FreeFloating;
            radioButton2.Placement = PlacementType.FreeFloating;

            // Flytta radioknappar inuti GroupBox
            radioButton1.Top = groupBox.Top + 20;
            radioButton1.Left = groupBox.Left + 20;
            radioButton2.Top = groupBox.Top + 50;
            radioButton2.Left = groupBox.Left + 20;

            // Visa GroupBox-egenskapsvärden efter gruppering
            Console.WriteLine("RadioButton1 GroupBox after grouping: " + radioButton1.GroupBox.Name);
            Console.WriteLine("RadioButton2 GroupBox after grouping: " + radioButton2.GroupBox.Name);

            // Demonstrera gruppbeteende
            radioButton1.IsChecked = true;
            Console.WriteLine("RadioButton1 checked state: " + radioButton1.IsChecked);
            Console.WriteLine("RadioButton2 checked state: " + radioButton2.IsChecked);

            // Spara resultatet
            workbook.Save("RadioButtonPropertyGroupBoxDemo.xlsx");
        }
    }
}
```

### Se även

* class [GroupBox](../../groupbox/)
* class [RadioButton](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


