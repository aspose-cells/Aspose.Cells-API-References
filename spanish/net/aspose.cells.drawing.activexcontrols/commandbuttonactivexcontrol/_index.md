---
title: "Clase CommandButtonActiveXControl"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.ActiveXControls.CommandButtonActiveXControl. Representa un botón de comando"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/
---
## CommandButtonActiveXControl class

Representa un botón de comando.

```csharp
public class CommandButtonActiveXControl : ActiveXControl
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Accelerator](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/accelerator/) { get; set; } | Obtiene y establece la tecla de acceso rápido para el control. |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Obtiene y establece el color ole del fondo.(Hereda de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Caption](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/caption/) { get; set; } | Obtiene y establece el texto descriptivo que aparece en un control. |
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
| [IsWordWrapped](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/iswordwrapped/) { get; set; } | Indica si el contenido del control se ajusta automáticamente al final de una línea. |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Obtiene y establece la celda vinculada.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Obtiene y establece el rango de llenado de la lista.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Obtiene y establece un ícono personalizado para mostrar como puntero del mouse del control.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Obtiene y establece el tipo de ícono que se muestra como puntero del mouse del control.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Picture](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/picture/) { get; set; } | Obtiene y establece los datos de la imagen. |
| [PicturePosition](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/pictureposition/) { get; set; } | Obtiene y establece la ubicación de la imagen del control relativa a su leyenda. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Indica si se muestra una sombra.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [TakeFocusOnClick](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/takefocusonclick/) { get; set; } | Indica si el control toma el foco al hacer clic. |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Representa cómo alinear el texto usado por el control.(Heredado de [`ActiveXControl`](../activexcontrol/).) |
| override [Type](../../aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/type/) { get; } | Obtiene el tipo del control ActiveX. |
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

    public class CommandButtonActiveXControlDemo
    {
        public static void CommandButtonActiveXControlExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue un control ActiveX CommandButton a la hoja de cálculo
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.CommandButton, 2, 2,2,2, 100, 30);
            CommandButtonActiveXControl commandButton = (CommandButtonActiveXControl)shape.ActiveXControl;

            // Establezca propiedades del control ActiveX CommandButton
            commandButton.Caption = "Click Me";
            commandButton.PicturePosition = ControlPicturePositionType.Center;
            commandButton.Accelerator = 'C';
            commandButton.TakeFocusOnClick = true;
            commandButton.IsWordWrapped = true;
            commandButton.IsEnabled = true;
            commandButton.IsLocked = false;
            commandButton.IsTransparent = false;
            commandButton.IsAutoSize = false;
            commandButton.IMEMode = InputMethodEditorMode.NoControl;
            commandButton.TextAlign = TextAlignmentType.Center;
            commandButton.Width = 150;
            commandButton.Height = 50;
            commandButton.MousePointer = ControlMousePointerType.Default;
            commandButton.ForeOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.Blue);
            commandButton.BackOleColor = System.Drawing.ColorTranslator.ToOle(System.Drawing.Color.LightGray);
            commandButton.IsVisible = true;
            commandButton.Shadow = true;
            commandButton.LinkedCell = "A1";
            commandButton.ListFillRange = "A2:A10";

            // Guarda el libro de trabajo
            workbook.Save("CommandButtonActiveXControlExample.xlsx");
            workbook.Save("CommandButtonActiveXControlExample.pdf");
        }
    }
}
```

### Ver también

* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


