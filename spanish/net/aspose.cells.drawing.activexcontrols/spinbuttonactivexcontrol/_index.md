---
title: "Clase SpinButtonActiveXControl"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.SpinButtonActiveXControl class. Representa el control SpinButton"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/
---
## SpinButtonActiveXControl class

Representa el control SpinButton.

```csharp
public class SpinButtonActiveXControl : ActiveXControl
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Obtiene y establece el color ole del fondo.(Hereda de [`ActiveXControlBase`](../activexcontrolbase/).) |
| override [Data](../../aspose.cells.drawing.activexcontrols/activexcontrol/data/) { get; } | Obtiene y establece los datos binarios del control.(Hereda de [`ActiveXControl`](../activexcontrol/).) |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | Representa la fuente del control.(Hereda de [`ActiveXControl`](../activexcontrol/).) |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Obtiene y establece el color ole del primer plano.(Hereda de [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Obtiene y establece la altura del control en unidades de puntos.(Hereda de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | Obtiene y establece el modo de ejecución predeterminado del Editor de Métodos de Entrada para el control cuando recibe el foco.(Hereda de [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsAutoSize](../../aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/) { get; set; } | Indica si el control redimensionará automáticamente para mostrar todo su contenido.(Hereda de [`ActiveXControl`](../activexcontrol/).) |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | Indica si el control puede recibir el foco y responder a eventos generados por el usuario.(Hereda de [`ActiveXControl`](../activexcontrol/).) |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | Indica si los datos del control están bloqueados para edición.(Hereda de [`ActiveXControl`](../activexcontrol/).) |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | Indica si el control es transparente.(Heredado de [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Indica si este control es visible.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Obtiene y establece la celda vinculada.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Obtiene y establece el rango de llenado de la lista.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Max](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/max/) { get; set; } | Obtiene y establece el valor máximo aceptable. |
| [Min](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/min/) { get; set; } | Obtiene y establece el valor mínimo aceptable. |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Obtiene y establece un ícono personalizado para mostrar como puntero del mouse del control.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Obtiene y establece el tipo de ícono que se muestra como puntero del mouse del control.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Orientation](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/orientation/) { get; set; } | Obtiene y establece si el SpinButton o ScrollBar está orientado vertical u horizontalmente. |
| [Position](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/position/) { get; set; } | Obtiene y establece el valor. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Indica si se muestra una sombra.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [SmallChange](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/smallchange/) { get; set; } | Obtiene y establece la cantidad en que cambia la propiedad Position |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Representa cómo alinear el texto usado por el control.(Heredado de [`ActiveXControl`](../activexcontrol/).) |
| override [Type](../../aspose.cells.drawing.activexcontrols/spinbuttonactivexcontrol/type/) { get; } | Obtiene el tipo del control ActiveX. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Obtiene y establece el ancho del control en unidades de puntos.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Obtiene el objeto [`Workbook`](../activexcontrolbase/workbook/).(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class SpinButtonActiveXControlDemo
    {
        public static void SpinButtonActiveXControlExample()
        {
            // Inicialice un nuevo libro de trabajo.
            Workbook workbook = new Workbook();

            // Agregar un SpinButtonActiveXControl.
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(ControlType.SpinButton, 1, 0, 1, 0, 100, 50);
            SpinButtonActiveXControl activeXControl = (SpinButtonActiveXControl)shape.ActiveXControl;

            // Estableciendo propiedades
            activeXControl.Min = 0;
            activeXControl.Max = 100;
            activeXControl.Position = 30;
            activeXControl.SmallChange = 5;

            if (activeXControl.Orientation == ControlScrollOrientation.Auto)
            {
                activeXControl.Orientation = ControlScrollOrientation.Horizontal;
            }

            activeXControl.IsEnabled = true;
            activeXControl.IsLocked = false;
            activeXControl.IsTransparent = false;
            activeXControl.IsAutoSize = true;
            activeXControl.IMEMode = InputMethodEditorMode.On;
            activeXControl.TextAlign = TextAlignmentType.Center;
            activeXControl.Width = 150;
            activeXControl.Height = 30;
            activeXControl.MousePointer = ControlMousePointerType.Default;
            activeXControl.ForeOleColor = 0x000000; // Black color
            activeXControl.BackOleColor = 0xFFFFFF; // White color
            activeXControl.IsVisible = true;
            activeXControl.Shadow = false;
            activeXControl.LinkedCell = "A1";
            activeXControl.ListFillRange = "A2:A10";

            // Guarda el libro de trabajo
            workbook.Save("SpinButtonActiveXControlExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


