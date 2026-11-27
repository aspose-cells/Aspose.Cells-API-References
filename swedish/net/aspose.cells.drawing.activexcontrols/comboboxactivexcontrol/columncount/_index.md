---
title: "ComboBoxActiveXControl.ColumnCount"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ComboBoxActiveXControl-egenskap. Representerar antalet kolumner som ska visas i en ComboBox eller ListBox"
type: docs
url: /sv/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/columncount/
---
## ComboBoxActiveXControl.ColumnCount property

Representerar antalet kolumner som ska visas i en ComboBox eller ListBox.

```csharp
public int ColumnCount { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyColumnCountDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Lägg till exempeldata
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Lägg till ComboBox ActiveX-kontroll
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 1, 0, 1, 0, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Ställ in ColumnCount-egenskapen och andra egenskaper
            comboBox.ColumnCount = 1;
            comboBox.ListWidth = 100;
            comboBox.Value = "Apple;Banana;Cherry";

            // Spara arbetsboken
            workbook.Save("ComboBoxColumnCountDemo.xlsx");

            Console.WriteLine("ComboBox with ColumnCount=1 has been created and saved.");
        }
    }
}
```

### Se även

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


