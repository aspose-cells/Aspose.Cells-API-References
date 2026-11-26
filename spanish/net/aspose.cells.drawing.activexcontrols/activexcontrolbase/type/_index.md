---
title: "ActiveXControlBase.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ActiveXControlBase. Obtiene el tipo del control ActiveX"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/type/
---
## ActiveXControlBase.Type property

Obtiene el tipo del control ActiveX.

```csharp
public abstract ControlType Type { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlBasePropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control Label ActiveX con los parámetros correctos
            Shape labelShape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 1, 1, 1, 100, 50, 0);
            LabelActiveXControl labelControl = (LabelActiveXControl)labelShape.ActiveXControl;
            labelControl.Caption = "Label_ActiveX";

            // Demostrar el uso de la propiedad Type
            if (labelShape.ActiveXControl.Type == ControlType.Label)
            {
                Console.WriteLine("The control is a Label type");
                labelControl.Caption = labelControl.Caption.Replace("Label_", "MyChangedLabel_");
            }

            // Guardar y verificar
            workbook.Save("output.xlsx");
            Console.WriteLine("Label caption changed to: " + labelControl.Caption);
        }
    }
}
```

### Ver también

* enum [ControlType](../../controltype/)
* class [ActiveXControlBase](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


