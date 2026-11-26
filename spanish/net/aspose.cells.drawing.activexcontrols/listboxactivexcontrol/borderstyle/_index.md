---
title: "ListBoxActiveXControl.BorderStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ListBoxActiveXControl propiedad. Obtiene y establece el tipo de borde utilizado por el control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/borderstyle/
---
## ListBoxActiveXControl.BorderStyle property

Obtiene y establece el tipo de borde utilizado por el control.

```csharp
public ControlBorderType BorderStyle { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyBorderStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega un control ListBox ActiveX con parámetros corregidos
            Shape shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 
                1, 0, 1, 100, 150, 30); // Added height parameter
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Establece la propiedad BorderStyle
            listBox.BorderStyle = ControlBorderType.None;

            // Verifica y muestra el estilo del borde
            Console.WriteLine("BorderStyle: " + listBox.BorderStyle);

            workbook.Save("ListBoxBorderStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ControlBorderType](../../controlbordertype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


