---
title: "Enum ShowDropButtonType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.ShowDropButtonType enum. Especifica cuándo mostrar el botón desplegable"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/showdropbuttontype/
---
## ShowDropButtonType enumeration

Especifica cuándo mostrar el botón desplegable

```csharp
public enum ShowDropButtonType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Never | `0` | Nunca mostrar el botón desplegable. |
| Focus | `1` | Mostrar el botón desplegable cuando el control tiene el foco. |
| Always | `2` | Mostrar siempre el botón desplegable. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ShowDropButtonTypeDemo
    {
        public static void ShowDropButtonTypeExample()
        {
            // Inicializa un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ComboBox a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 1, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Establecer propiedades para el control ActiveX ComboBox
            comboBox.ShowDropButtonTypeWhen = ShowDropButtonType.Focus; // Show drop button when the control has focus
            comboBox.ListWidth = 100;
            comboBox.ListRows = 5;
            comboBox.IsEditable = true;

            // Agregar algunos elementos al ComboBox
            comboBox.LinkedCell = "A1";
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Guarda el libro de trabajo
            workbook.Save("ShowDropButtonTypeExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


