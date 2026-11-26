---
title: "Enum ControlSpecialEffectType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.ActiveXControls.ControlSpecialEffectType. Representa el tipo de efecto especial"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/controlspecialeffecttype/
---
## ControlSpecialEffectType enumeration

Representa el tipo de efecto especial.

```csharp
public enum ControlSpecialEffectType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Flat | `0` | Plano |
| Raised | `1` | Elevado |
| Sunken | `2` | Hundido |
| Etched | `3` | Grabado |
| Bump | `6` | Abultado |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlSpecialEffectTypeDemo
    {
        public static void ControlSpecialEffectTypeExample()
        {
            // Inicializa un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX CheckBox
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 1, 0, 1, 0, 100, 50);
            CheckBoxActiveXControl checkBoxControl = (CheckBoxActiveXControl)shape.ActiveXControl;

            // Establecer propiedades del control ActiveX CheckBox
            checkBoxControl.Caption = "Example CheckBox";
            checkBoxControl.SpecialEffect = ControlSpecialEffectType.Raised;

            // Agregar un control ActiveX ComboBox
            shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 3, 0, 3, 0, 100, 50);
            ComboBoxActiveXControl comboBoxControl = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Establecer propiedades del control ActiveX ComboBox
            comboBoxControl.SpecialEffect = ControlSpecialEffectType.Sunken;
            comboBoxControl.ListWidth = 100;
            comboBoxControl.ListRows = 5;

            // Agregar un control ActiveX TextBox
            shape = worksheet.Shapes.AddActiveXControl(ControlType.TextBox, 5, 0, 5, 0, 100, 50);
            TextBoxActiveXControl textBoxControl = (TextBoxActiveXControl)shape.ActiveXControl;

            // Establecer propiedades del control ActiveX TextBox
            textBoxControl.Text = "Example TextBox";
            textBoxControl.SpecialEffect = ControlSpecialEffectType.Bump;

            // Guarda el libro de trabajo
            workbook.Save("ControlSpecialEffectTypeExample.xlsx");
            workbook.Save("ControlSpecialEffectTypeExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


