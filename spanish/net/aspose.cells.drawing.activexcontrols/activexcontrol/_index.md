---
title: "Clase ActiveXControl"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.ActiveXControls.ActiveXControl. Representa el control ActiveX"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/activexcontrol/
---
## ActiveXControl class

Representa el control ActiveX.

```csharp
public abstract class ActiveXControl : ActiveXControlBase
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Obtiene y establece el color ole del fondo.(Hereda de [`ActiveXControlBase`](../activexcontrolbase/).) |
| override [Data](../../aspose.cells.drawing.activexcontrols/activexcontrol/data/) { get; } | Obtiene y establece los datos binarios del control. |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | Representa la fuente del control. |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Obtiene y establece el color ole del primer plano.(Hereda de [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Obtiene y establece la altura del control en unidades de puntos.(Hereda de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | Obtiene y establece el modo de tiempo de ejecución predeterminado del Editor de Métodos de Entrada para el control cuando recibe el foco. |
| virtual [IsAutoSize](../../aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/) { get; set; } | Indica si el control cambiará de tamaño automáticamente para mostrar todo su contenido. |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | Indica si el control puede recibir el foco y responder a eventos generados por el usuario. |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | Indica si los datos del control están bloqueados para edición. |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | Indica si el control es transparente. |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Indica si este control es visible.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Obtiene y establece la celda vinculada.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Obtiene y establece el rango de llenado de la lista.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Obtiene y establece un ícono personalizado para mostrar como puntero del mouse del control.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Obtiene y establece el tipo de ícono que se muestra como puntero del mouse del control.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Indica si se muestra una sombra.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Representa cómo alinear el texto usado por el control. |
| abstract [Type](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/type/) { get; } | Obtiene el tipo del control ActiveX. (Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Obtiene y establece el ancho del control en unidades de puntos.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Obtiene el objeto [`Workbook`](../activexcontrolbase/workbook/).(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ActiveXControlsClassActiveXControlDemo
    {
        public static void Run()
        {
            // Crear libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar control ActiveX RadioButton
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.RadioButton, 
                1, 1,  // upper left row/column
                1, 1,  // upper left row/column offsets
                100, 30);  // width and height
            RadioButtonActiveXControl radioButton = (RadioButtonActiveXControl)shape.ActiveXControl;

            // Establecer propiedades
            radioButton.GroupName = "Sheet1";
            radioButton.Alignment = ControlCaptionAlignmentType.Left;
            radioButton.IsWordWrapped = true;
            radioButton.Caption = "OptionButton1";
            radioButton.PicturePosition = ControlPicturePositionType.AboveCenter;
            radioButton.SpecialEffect = ControlSpecialEffectType.Sunken;
            radioButton.IsEnabled = true;
            radioButton.IsTransparent = false;
            radioButton.IsAutoSize = false;
            radioButton.IMEMode = InputMethodEditorMode.NoControl;
            radioButton.Font.Name = "Calibri";
            radioButton.MousePointer = ControlMousePointerType.Default;

            // Guarda el libro de trabajo
            workbook.Save("ActiveXControlDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ActiveXControlBase](../activexcontrolbase/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


