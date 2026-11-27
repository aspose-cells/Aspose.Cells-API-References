---
title: "ComboBoxActiveXControl.ShowColumnHeads"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ComboBoxActiveXControl-egenskap. Anger om kolumnrubriker visas"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/showcolumnheads/
---
## ComboBoxActiveXControl.ShowColumnHeads property

Anger om kolumnrubriker visas.

```csharp
public bool ShowColumnHeads { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyShowColumnHeadsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till en ComboBox ActiveX-kontroll
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 1, 0, 1, 0, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Ange egenskaper för ComboBox
            comboBox.ColumnCount = 2;
            comboBox.ListWidth = 100;
            
            // Lägg till exempeldata i ComboBoxen
            comboBox.ListFillRange = "A1:B3";
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue("Value1");
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue("Value2");

            // Demonstrera egenskapen ShowColumnHeads
            Console.WriteLine("Initial ShowColumnHeads value: " + comboBox.ShowColumnHeads);
            
            // Aktivera kolumnrubriker
            comboBox.ShowColumnHeads = true;
            Console.WriteLine("After setting ShowColumnHeads to true: " + comboBox.ShowColumnHeads);
            
            // Inaktivera kolumnrubriker
            comboBox.ShowColumnHeads = false;
            Console.WriteLine("After setting ShowColumnHeads to false: " + comboBox.ShowColumnHeads);

            // Spara arbetsboken
            workbook.Save("ComboBoxShowColumnHeadsDemo.xlsx");
        }
    }
}
```

### Se även

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


