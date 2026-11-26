---
title: "Enum ControlType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ControlType enum. Representa todos los tipos de control ActiveX"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/controltype/
---
## ControlType enumeration

Representa todos los tipos de control ActiveX.

```csharp
public enum ControlType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| CommandButton | `0` | Botón |
| ComboBox | `1` | ComboBox |
| CheckBox | `2` | CheckBox |
| ListBox | `3` | ListBox |
| TextBox | `4` | TextBox |
| SpinButton | `5` | Spinner |
| RadioButton | `6` | RadioButton |
| Label | `7` | Etiqueta |
| Image | `8` | Imagen |
| ToggleButton | `9` | ToggleButton |
| ScrollBar | `10` | ScrollBar |
| BarCode | `11` | ScrollBar |
| Unknown | `12` | Desconocido |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlTypeDemo
    {
        public static void ControlTypeExample()
        {
            // Inicializa un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX CommandButton
            Shape commandButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 1, 0, 1, 0, 100, 30);
            ActiveXControl commandButtonControl = commandButtonShape.ActiveXControl;
            commandButtonControl.IsEnabled = true;
            commandButtonControl.IsVisible = true;

            // Agregar un control ActiveX ComboBox
            Shape comboBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 3, 0, 1, 0, 100, 30);
            ActiveXControl comboBoxControl = comboBoxShape.ActiveXControl;
            comboBoxControl.IsEnabled = true;
            comboBoxControl.IsVisible = true;

            // Agregar un control ActiveX CheckBox
            Shape checkBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 1, 0, 100, 30);
            ActiveXControl checkBoxControl = checkBoxShape.ActiveXControl;
            checkBoxControl.IsEnabled = true;
            checkBoxControl.IsVisible = true;

            // Agregar un control ActiveX ListBox
            Shape listBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 7, 0, 1, 0, 100, 30);
            ActiveXControl listBoxControl = listBoxShape.ActiveXControl;
            listBoxControl.IsEnabled = true;
            listBoxControl.IsVisible = true;

            // Agregar un control ActiveX TextBox
            Shape textBoxShape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 9, 0, 1, 0, 100, 30);
            ActiveXControl textBoxControl = textBoxShape.ActiveXControl;
            textBoxControl.IsEnabled = true;
            textBoxControl.IsVisible = true;

            // Agregar un control ActiveX SpinButton
            Shape spinButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.SpinButton, 11, 0, 1, 0, 100, 30);
            ActiveXControl spinButtonControl = spinButtonShape.ActiveXControl;
            spinButtonControl.IsEnabled = true;
            spinButtonControl.IsVisible = true;

            // Agregar un control ActiveX RadioButton
            Shape radioButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.RadioButton, 13, 0, 1, 0, 100, 30);
            ActiveXControl radioButtonControl = radioButtonShape.ActiveXControl;
            radioButtonControl.IsEnabled = true;
            radioButtonControl.IsVisible = true;

            // Agregar un control ActiveX Label
            Shape labelShape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 15, 0, 1, 0, 100, 30);
            ActiveXControl labelControl = labelShape.ActiveXControl;
            labelControl.IsEnabled = true;
            labelControl.IsVisible = true;

            // Agregar un control ActiveX Image
            Shape imageShape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 17, 0, 1, 0, 100, 30);
            ActiveXControl imageControl = imageShape.ActiveXControl;
            imageControl.IsEnabled = true;
            imageControl.IsVisible = true;

            // Agregar un control ActiveX ToggleButton
            Shape toggleButtonShape = worksheet.Shapes.AddActiveXControl(ControlType.ToggleButton, 19, 0, 1, 0, 100, 30);
            ActiveXControl toggleButtonControl = toggleButtonShape.ActiveXControl;
            toggleButtonControl.IsEnabled = true;
            toggleButtonControl.IsVisible = true;

            // Agregar un control ActiveX ScrollBar
            Shape scrollBarShape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 21, 0, 1, 0, 100, 30);
            ActiveXControl scrollBarControl = scrollBarShape.ActiveXControl;
            scrollBarControl.IsEnabled = true;
            scrollBarControl.IsVisible = true;
                       

            // Guarda el libro de trabajo
            workbook.Save("ControlTypeExample.xlsx");
            workbook.Save("ControlTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


