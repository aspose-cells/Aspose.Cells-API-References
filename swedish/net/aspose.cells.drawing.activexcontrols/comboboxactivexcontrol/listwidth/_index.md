---
title: "ComboBoxActiveXControl.ListWidth"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ComboBoxActiveXControl-egenskap. Hämtar och sätter bredden i enheten punkter"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/listwidth/
---
## ComboBoxActiveXControl.ListWidth property

Hämtar och anger bredden i enheter av punkter.

```csharp
public double ListWidth { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyListWidthDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata för ComboBox
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");

            // Lägg till en ComboBox ActiveX control med alla nödvändiga parametrar
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox,
                1,  // left
                1,  // top
                100, // width
                30,  // height
                0,   // image width (unused for ComboBox)
                0    // image height (unused for ComboBox)
            );
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Ställ in ListWidth-egenskapen för att kontrollera rullgardinsbredden
            comboBox.ListWidth = 150;
            comboBox.ListRows = 3;
            comboBox.LinkedCell = "A1:A3";

            // Spara arbetsboken
            workbook.Save("ComboBoxListWidthDemo.xlsx");

            Console.WriteLine("ComboBox ListWidth set to: " + comboBox.ListWidth);
        }
    }
}
```

### Se även

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


