---
title: "ListBoxActiveXControl.Value"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ListBoxActiveXControl-egenskap. Hämtar och anger kontrollens värde"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/value/
---
## ListBoxActiveXControl.Value property

Hämtar och anger värdet för kontrollen.

```csharp
public string Value { get; set; }
```

### Anmärkningar

Endast effekt när [`SelectionType`](../selectiontype/) är SelectionType.Single;

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ListBox ActiveX-kontroll
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 1, 0, 1, 0, 100, 60);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Ställ in grundläggande egenskaper
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;

            // Ställ in objekt med Value‑egenskap
            listBox.Value = "Red;Green;Blue;Yellow";

            // Spara arbetsboken
            workbook.Save("ListBoxValueDemo.xlsx");

            Console.WriteLine("ListBox with items set using Value property has been created.");
        }
    }
}
```

### Se även

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


