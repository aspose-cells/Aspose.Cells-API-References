---
title: "ComboBoxActiveXControl.ListStyle"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ComboBoxActiveXControl egenskap. Hämtar och anger det visuella utseendet"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/liststyle/
---
## ComboBoxActiveXControl.ListStyle property

Hämtar och anger det visuella utseendet.

```csharp
public ControlListStyle ListStyle { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyListStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Items");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");

            // Lägg till ComboBox med vanlig liststil
            var comboBoxShape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 1, 0, 1, 0, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)comboBoxShape.ActiveXControl;
            comboBox.ListStyle = Aspose.Cells.Drawing.ActiveXControls.ControlListStyle.Plain;
            comboBox.ListFillRange = "A2:A4";

            // Lägg till ListBox med alternativliststil
            var listBoxShape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 0, 100, 60);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)listBoxShape.ActiveXControl;
            listBox.ListStyle = Aspose.Cells.Drawing.ActiveXControls.ControlListStyle.Option;
            listBox.ListFillRange = "A2:A4";

            // Spara och demonstrera
            workbook.Save("ListStyleDemo.xlsx");
            Console.WriteLine("ComboBox ListStyle: " + comboBox.ListStyle);
            Console.WriteLine("ListBox ListStyle: " + listBox.ListStyle);
        }
    }
}
```

### Se även

* enum [ControlListStyle](../../controlliststyle/)
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


