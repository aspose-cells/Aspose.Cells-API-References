---
title: "Enumeración ControlScrollOrientation"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.ActiveXControls.ControlScrollOrientation. Representa el tipo de orientación de desplazamiento"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/controlscrollorientation/
---
## ControlScrollOrientation enumeration

Representa el tipo de orientación de desplazamiento

```csharp
public enum ControlScrollOrientation
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Auto | `3` | El control se muestra horizontalmente cuando el ancho del control es mayor que su altura. De lo contrario, el control se muestra verticalmente. |
| Vertical | `0` | El control se muestra verticalmente. |
| Horizontal | `1` | El control se muestra horizontalmente. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlScrollOrientationDemo
    {
        public static void ControlScrollOrientationExample()
        {
            // Inicializa un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregue un ScrollBarActiveXControl a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ScrollBar, 1, 0, 1, 0, 100, 50);
            ScrollBarActiveXControl activeXControl = (ScrollBarActiveXControl)shape.ActiveXControl;

            // Establezca propiedades para el ScrollBarActiveXControl
            activeXControl.LargeChange = 5;
            activeXControl.Min = 0;
            activeXControl.Max = 100;
            activeXControl.Position = 30;
            activeXControl.SmallChange = 5;

            // Demuestre la configuración de la orientación usando la enumeración ControlScrollOrientation
            if (activeXControl.Orientation == ControlScrollOrientation.Auto)
            {
                activeXControl.Orientation = ControlScrollOrientation.Horizontal;
            }

            // Guarda el libro de trabajo
            workbook.Save("ControlScrollOrientationExample.xlsx");
            workbook.Save("ControlScrollOrientationExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


