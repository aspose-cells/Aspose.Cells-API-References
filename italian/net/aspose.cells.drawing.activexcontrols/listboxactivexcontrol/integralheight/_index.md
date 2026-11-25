---
title: "ListBoxActiveXControl.IntegralHeight"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ListBoxActiveXControl. Indica se il controllo mostrerà solo linee di testo complete senza visualizzare linee parziali"
type: docs
url: /it/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/integralheight/
---
## ListBoxActiveXControl.IntegralHeight property

Indica se il controllo mostrerà solo linee complete di testo senza visualizzare linee parziali.

```csharp
public bool IntegralHeight { get; set; }
```

### Esempi

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyIntegralHeightDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,
                10,  // left
                10,  // top
                200, // width
                100, // height
                0,   // imageWidth (required parameter)
                0    // imageHeight (required parameter)
            );
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Dimostra la proprietà IntegralHeight
            listBox.IntegralHeight = true;
            Console.WriteLine("ListBox IntegralHeight set to: " + listBox.IntegralHeight);

            // Aggiungi elementi di esempio
            listBox.ListFillRange = "A1:A3";
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");

            workbook.Save("ListBoxIntegralHeightDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


