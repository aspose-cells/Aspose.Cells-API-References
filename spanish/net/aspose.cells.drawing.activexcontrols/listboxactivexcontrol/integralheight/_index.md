---
title: "ListBoxActiveXControl.IntegralHeight"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ListBoxActiveXControl propiedad. Indica si el control solo mostrará líneas completas de texto sin mostrar líneas parciales"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/integralheight/
---
## ListBoxActiveXControl.IntegralHeight property

Indica si el control solo mostrará líneas completas de texto sin mostrar líneas parciales.

```csharp
public bool IntegralHeight { get; set; }
```

### Ejemplos

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

            // Demuestra la propiedad IntegralHeight
            listBox.IntegralHeight = true;
            Console.WriteLine("ListBox IntegralHeight set to: " + listBox.IntegralHeight);

            // Agrega elementos de muestra
            listBox.ListFillRange = "A1:A3";
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");

            workbook.Save("ListBoxIntegralHeightDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


