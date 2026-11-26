---
title: "RadioButtonActiveXControl.GroupName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad RadioButtonActiveXControl. Obtiene y establece el nombre del grupo"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/radiobuttonactivexcontrol/groupname/
---
## RadioButtonActiveXControl.GroupName property

Obtiene y establece el nombre del grupo.

```csharp
public string GroupName { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RadioButtonActiveXControlPropertyGroupNameDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar dos controles RadioButton ActiveX
            var shape1 = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 0, 100, 30);
            var radio1 = (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape1.ActiveXControl;
            
            var shape2 = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.RadioButton, 1, 0, 1, 50, 100, 30);
            var radio2 = (Aspose.Cells.Drawing.ActiveXControls.RadioButtonActiveXControl)shape2.ActiveXControl;

            // Establecer el mismo nombre de grupo para que sean mutuamente excluyentes
            radio1.GroupName = "RadioGroup1";
            radio2.GroupName = "RadioGroup1";

            // Establecer leyendas
            radio1.Caption = "Option 1";
            radio2.Caption = "Option 2";

            // Guarda el libro de trabajo
            workbook.Save("RadioButtonGroupDemo.xlsx");
        }
    }
}
```

### Ver también

* class [RadioButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


