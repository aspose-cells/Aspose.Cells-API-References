---
title: "Enum ControlCaptionAlignmentType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlCaptionAlignmentType enum. Representa la posición del Caption respecto al control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/controlcaptionalignmenttype/
---
## ControlCaptionAlignmentType enumeration

Representa la posición del título relativo al control.

```csharp
public enum ControlCaptionAlignmentType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Left | `0` | El lado izquierdo del control. |
| Right | `1` | El lado derecho del control. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlCaptionAlignmentTypeDemo
    {
        public static void ControlCaptionAlignmentTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX CheckBox a la hoja de cálculo
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 1, 1, 100, 20);
            CheckBoxActiveXControl checkBox = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Establecer propiedades para el CheckBox
            checkBox.Caption = "Check Me!";
            checkBox.Alignment = ControlCaptionAlignmentType.Right;
            checkBox.IsWordWrapped = true;
            checkBox.Value = CheckValueType.Checked;

            // Agregar un control ActiveX RadioButton a la hoja de cálculo
            var shape2 = worksheet.Shapes.AddActiveXControl(ControlType.RadioButton, 10, 0, 1, 1, 100, 20);
            RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape2.ActiveXControl;

            // Establecer propiedades para el RadioButton
            radioButton.Caption = "Select Me!";
            radioButton.Alignment = ControlCaptionAlignmentType.Left;
            radioButton.IsWordWrapped = true;

            // Guarda el libro de trabajo
            workbook.Save("ControlCaptionAlignmentTypeExample.xlsx");
            workbook.Save("ControlCaptionAlignmentTypeExample.pdf");
            // Genere la salida de los resultados
            Console.WriteLine("CheckBox Alignment: " + checkBox.Alignment);
            Console.WriteLine("RadioButton Alignment: " + radioButton.Alignment);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


