---
title: "CheckBoxActiveXControl.GroupName"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CheckBoxActiveXControl. Obtiene y establece el nombre del grupo"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/groupname/
---
## CheckBoxActiveXControl.GroupName property

Obtiene y establece el nombre del grupo.

```csharp
public string GroupName { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyGroupNameDemo
    {
        public static void Run()
        {
            // Crear libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX CheckBox
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 1, 1, 1, 100, 50);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Establecer la propiedad GroupName
            checkBox.GroupName = "Sheet1";

            // Verificar y mostrar el GroupName
            Console.WriteLine("CheckBox GroupName: " + checkBox.GroupName);

            // Guarda el libro de trabajo
            workbook.Save("CheckBoxActiveXControlGroupNameDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


