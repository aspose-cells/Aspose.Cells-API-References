---
title: "ComboBoxActiveXControl.Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ComboBoxActiveXControl-egenskap. Hämtar och anger värdet för kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/value/
---
## ComboBoxActiveXControl.Value property

Hämtar och anger värdet för kontrollen.

```csharp
public string Value { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ComboBox ActiveX-kontroll i kalkylbladet
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 1, 1, 0, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Ange egenskaper för ComboBox
            comboBox.Value = "Initial Value";
            comboBox.ListFillRange = "A1:A3";
            
            // Lägg till exempeldata i listområdet
            worksheet.Cells["A1"].PutValue("Option 1");
            worksheet.Cells["A2"].PutValue("Option 2");
            worksheet.Cells["A3"].PutValue("Option 3");

            // Uppdatera det valda värdet från länkad cell
            worksheet.Cells["B1"].PutValue("Option 2");
            worksheet.Shapes.UpdateSelectedValue();

            // Demonstrera hämtning av Value-egenskapen
            Console.WriteLine("ComboBox Value: " + comboBox.Value);

            // Spara arbetsboken
            workbook.Save("ComboBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Se även

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


