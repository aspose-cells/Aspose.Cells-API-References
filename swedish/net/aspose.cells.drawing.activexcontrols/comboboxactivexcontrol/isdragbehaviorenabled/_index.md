---
title: "ComboBoxActiveXControl.IsDragBehaviorEnabled"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ComboBoxActiveXControl-egenskap. Anger om dra‑och‑släpp är aktiverat för kontrollen"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/isdragbehaviorenabled/
---
## ComboBoxActiveXControl.IsDragBehaviorEnabled property

Indikerar om dra och släpp är aktiverat för kontrollen.

```csharp
public bool IsDragBehaviorEnabled { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyIsDragBehaviorEnabledDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ComboBox ActiveX-kontroll
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 1, 0, 1, 0, 100, 50);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Ställ in några grundläggande egenskaper
            comboBox.ListRows = 8;
            comboBox.ColumnCount = 1;
            comboBox.BoundColumn = 1;
            comboBox.TextColumn = -1;

            // Demonstrera egenskapen IsDragBehaviorEnabled
            Console.WriteLine("Initial IsDragBehaviorEnabled: " + comboBox.IsDragBehaviorEnabled);
            
            // Inaktivera dragbeteende
            comboBox.IsDragBehaviorEnabled = false;
            Console.WriteLine("After setting to false: " + comboBox.IsDragBehaviorEnabled);
            
            // Aktivera dragbeteende
            comboBox.IsDragBehaviorEnabled = true;
            Console.WriteLine("After setting to true: " + comboBox.IsDragBehaviorEnabled);

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


