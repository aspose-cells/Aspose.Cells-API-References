---
title: "CheckBoxActiveXControl.Caption"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CheckBoxActiveXControl. Obtiene y establece el texto descriptivo que aparece en un control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/caption/
---
## CheckBoxActiveXControl.Caption property

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
    public class CheckBoxActiveXControlPropertyCaptionDemo
    {
        public static void Run()
        {
            // Inicializa un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX CheckBox
            Shape shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.CheckBox, 1, 0, 1, 0, 100, 50);
            CheckBoxActiveXControl checkBoxControl = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Establecer y demostrar la propiedad Caption
            checkBoxControl.Caption = "Sample CheckBox Caption";
            checkBoxControl.Value = CheckValueType.Checked;  // Fixed: Using correct enum value

            // Guarda el libro de trabajo
            workbook.Save("CheckBoxCaptionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


