---
title: "Enum ControlBorderType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.ActiveXControls.ControlBorderType. Representa el tipo de borde del control ActiveX"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/controlbordertype/
---
## ControlBorderType enumeration

Representa el tipo de borde del control ActiveX.

```csharp
public enum ControlBorderType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Sin borde. |
| Single | `1` | La línea única. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;

    public class ControlBorderTypeDemo
    {
        public static void ControlBorderTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ComboBox a la hoja de cálculo
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Establecer propiedades para el control ActiveX ComboBox
            comboBox.MaxLength = 100;
            comboBox.ListWidth = 150;
            comboBox.BoundColumn = 1;
            comboBox.TextColumn = 1;
            comboBox.ColumnCount = 1;
            comboBox.ListRows = 5;
            comboBox.MatchEntry = ControlMatchEntryType.Complete;
            comboBox.DropButtonStyle = DropButtonStyle.Arrow;
            comboBox.ShowDropButtonTypeWhen = ShowDropButtonType.Always;
            comboBox.ListStyle = ControlListStyle.Plain;
            comboBox.BorderStyle = ControlBorderType.Single; // Set border style to Single
            comboBox.BorderOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Black);
            comboBox.SpecialEffect = ControlSpecialEffectType.Flat;
            comboBox.IsEditable = true;
            comboBox.ShowColumnHeads = false;
            comboBox.IsDragBehaviorEnabled = false;
            comboBox.EnterFieldBehavior = true;
            comboBox.IsAutoWordSelected = false;
            comboBox.SelectionMargin = false;
            comboBox.Value = "Sample Text";
            comboBox.HideSelection = true;
            comboBox.ColumnWidths = 100;

            // Guarda el libro de trabajo
            workbook.Save("ControlBorderTypeExample.xlsx");
            workbook.Save("ControlBorderTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


