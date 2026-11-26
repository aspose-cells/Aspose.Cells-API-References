---
title: "Enumeración ControlScrollBarType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.ActiveXControls.ControlScrollBarType. Representa el tipo de barra de desplazamiento"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/controlscrollbartype/
---
## ControlScrollBarType enumeration

Representa el tipo de barra de desplazamiento.

```csharp
public enum ControlScrollBarType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | No muestra barras de desplazamiento. |
| Horizontal | `1` | Muestra una barra de desplazamiento horizontal. |
| BarsVertical | `2` | Muestra una barra de desplazamiento vertical. |
| BarsBoth | `3` | Muestra tanto una barra de desplazamiento horizontal como una vertical. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ControlScrollBarTypeDemo
    {
        public static void ControlScrollBarTypeExample()
        {
            // Inicializa un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ListBox a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ListBox, 1, 0, 1, 0, 100, 50);
            ListBoxActiveXControl listBoxControl = (ListBoxActiveXControl)shape.ActiveXControl;

            // Establezca la propiedad ScrollBars para mostrar tanto barras de desplazamiento horizontales como verticales
            listBoxControl.ScrollBars = ControlScrollBarType.BarsBoth;

            // Guarda el libro de trabajo
            workbook.Save("ControlScrollBarTypeExample.xlsx");
            workbook.Save("ControlScrollBarTypeExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


