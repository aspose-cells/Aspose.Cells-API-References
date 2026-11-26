---
title: "CheckBoxActiveXControl.PicturePosition"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CheckBoxActiveXControl. Obtiene y establece la ubicación de la imagen del control relativa a su título"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/checkboxactivexcontrol/pictureposition/
---
## CheckBoxActiveXControl.PicturePosition property

Obtiene y establece la ubicación de la imagen del control relativa a su leyenda.

```csharp
public ControlPicturePositionType PicturePosition { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CheckBoxActiveXControlPropertyPicturePositionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control CheckBox ActiveX con todos los parámetros requeridos
            var shape = worksheet.Shapes.AddActiveXControl(
                ControlType.CheckBox, 
                10,  // left
                10,  // top
                150, // width
                30,  // height
                0,   // leftOffset
                0    // topOffset
            );
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Configurar las propiedades del CheckBox
            checkBox.Caption = "Sample CheckBox";
            checkBox.PicturePosition = ControlPicturePositionType.Center;
            checkBox.IsAutoSize = true;

            // Guarda el libro de trabajo
            workbook.Save("CheckBoxPicturePositionDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ControlPicturePositionType](../../controlpicturepositiontype/)
* class [CheckBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


