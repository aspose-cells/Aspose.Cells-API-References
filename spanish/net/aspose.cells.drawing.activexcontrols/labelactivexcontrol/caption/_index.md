---
title: "LabelActiveXControl.Caption"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LabelActiveXControl. Obtiene y establece el texto descriptivo que aparece en un control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/caption/
---
## LabelActiveXControl.Caption property

Obtiene y establece el texto descriptivo que aparece en un control.

```csharp
public string Caption { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyCaptionDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar control ActiveX Label
            Shape shape = sheet.Shapes.AddActiveXControl(ControlType.Label, 0, 0, 0, 0, 100, 30);
            LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

            // Establecer y demostrar la propiedad Caption
            label.Caption = "Label1aaaa";
            
            // Guardar y recargar para verificar la persistencia
            string path = "LabelActiveXDemo.xlsm";
            workbook.Save(path, SaveFormat.Xlsm);

            Workbook reopened = new Workbook(path);
            LabelActiveXControl reloadedLabel = (LabelActiveXControl)reopened.Worksheets[0].Shapes[0].ActiveXControl;
            Console.WriteLine("Caption: " + reloadedLabel.Caption);
        }
    }
}
```

### Ver también

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


