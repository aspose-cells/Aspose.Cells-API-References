---
title: "Enum DropButtonStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.DropButtonStyle enum. Representa el símbolo que se muestra en el botón desplegable"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/dropbuttonstyle/
---
## DropButtonStyle enumeration

Representa el símbolo mostrado en el botón desplegable.

```csharp
public enum DropButtonStyle
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Plain | `0` | Muestra un botón sin símbolo. |
| Arrow | `1` | Muestra un botón con una flecha hacia abajo. |
| Ellipsis | `2` | Muestra un botón con una elipsis (...). |
| Reduce | `3` | Muestra un botón con una línea horizontal similar a un carácter de subrayado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class DropButtonStyleDemo
    {
        public static void DropButtonStyleExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ComboBox a la hoja de cálculo
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 1, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Establecer propiedades para el ComboBox
            comboBox.ListWidth = 100;
            comboBox.ListRows = 5;
            comboBox.ColumnCount = 1;
            comboBox.DropButtonStyle = DropButtonStyle.Arrow; // Set the drop button style to Arrow

            // Agregar algunos elementos al ComboBox
            comboBox.LinkedCell = "A1";
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            comboBox.ListFillRange = "A1:A4";

            // Guarda el libro de trabajo
            workbook.Save("DropButtonStyleExample.xlsx");
            workbook.Save("DropButtonStyleExample.pdf");

            // Mostrar el DropButtonStyle utilizado
            Console.WriteLine("DropButtonStyle set to: " + comboBox.DropButtonStyle);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


