---
title: "Clase ActiveXControlBase"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.ActiveXControls.ActiveXControlBase. Representa el control ActiveX"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/activexcontrolbase/
---
## ActiveXControlBase class

Representa el control ActiveX.

```csharp
public abstract class ActiveXControlBase
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Obtiene y establece el color ole del fondo. |
| virtual [Data](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/data/) { get; } | Obtiene y establece los datos binarios del control. |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Obtiene y establece el color OLE del primer plano. |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Obtiene y establece la altura del control en unidades de puntos. |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Indica si este control es visible. |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Obtiene y establece la celda vinculada. |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Obtiene y establece el rango de relleno de la lista. |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Obtiene y establece un ícono personalizado para mostrar como puntero del mouse para el control. |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Obtiene y establece el tipo de ícono que se muestra como puntero del mouse para el control. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Indica si se debe mostrar una sombra. |
| abstract [Type](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/type/) { get; } | Obtiene el tipo del control ActiveX. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Obtiene y establece el ancho del control en unidades de puntos. |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Obtiene el objeto [`Workbook`](./workbook/). |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlBaseDemo
    {
        public static void ActiveXControlBaseExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX a la hoja de cálculo
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CheckBox, 5, 0, 5, 0, 100, 20);

            CheckBoxActiveXControl control = (CheckBoxActiveXControl)shape.ActiveXControl;
            control.Font.Size = 20;

            // Establecer propiedades del control ActiveX
            control.Width = 150;
            control.Height = 30;
            control.MousePointer = ControlMousePointerType.Arrow;
            control.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Red);
            control.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Yellow);
            control.IsVisible = true;
            control.Shadow = true;
            control.LinkedCell = "A1";
            control.ListFillRange = "A2:A10";

            // Guarda el libro de trabajo
            workbook.Save("ActiveXControlBaseExample.xlsx");
            workbook.Save("ActiveXControlBaseExample.pdf", SaveFormat.Pdf);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


