---
title: "TextBoxActiveXControl.ShowDropButtonTypeWhen"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TextBoxActiveXControl. Especifica el símbolo que se muestra en el botón desplegable"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/showdropbuttontypewhen/
---
## TextBoxActiveXControl.ShowDropButtonTypeWhen property

Especifica el símbolo mostrado en el botón desplegable

```csharp
public ShowDropButtonType ShowDropButtonTypeWhen { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class TextBoxActiveXControlPropertyShowDropButtonTypeWhenDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX TextBox
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.TextBox, 
                1, 1, 1, 1, 100, 50);
            TextBoxActiveXControl textBox = (TextBoxActiveXControl)shape.ActiveXControl;

            // Establecer la propiedad ShowDropButtonTypeWhen
            textBox.ShowDropButtonTypeWhen = ShowDropButtonType.Focus;

            // Guarda el libro de trabajo
            workbook.Save("TextBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ShowDropButtonType](../../showdropbuttontype/)
* class [TextBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


