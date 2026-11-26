---
title: "Clase TextBoxActiveXControl"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Drawing.ActiveXControls.TextBoxActiveXControl class. Representa un control ActiveX de cuadro de texto"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/textboxactivexcontrol/
---
## TextBoxActiveXControl class

Representa un control ActiveX de cuadro de texto.

```csharp
public class TextBoxActiveXControl : ActiveXControl
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Obtiene y establece el color ole del fondo.(Hereda de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [BorderOleColor](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/borderolecolor/) { get; set; } | Obtiene y establece el color ole del fondo. |
| [BorderStyle](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/borderstyle/) { get; set; } | Obtiene y establece el tipo de borde utilizado por el control. |
| override [Data](../../aspose.cells.drawing.activexcontrols/activexcontrol/data/) { get; } | Obtiene y establece los datos binarios del control.(Hereda de [`ActiveXControl`](../activexcontrol/).) |
| [DropButtonStyle](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/dropbuttonstyle/) { get; set; } | Especifica el símbolo mostrado en el botón desplegable |
| [EnterFieldBehavior](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/enterfieldbehavior/) { get; set; } | Especifica el comportamiento de selección al entrar al control. True indica que la selección permanece sin cambios desde la última vez que el control estuvo activo. False indica que todo el texto del control se seleccionará al entrar al control. |
| [EnterKeyBehavior](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/enterkeybehavior/) { get; set; } | Especifica el comportamiento de la tecla ENTER. True especifica que al presionar ENTER se creará una nueva línea. False especifica que al presionar ENTER se moverá el foco al siguiente objeto en el orden de tabulación. |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | Representa la fuente del control.(Hereda de [`ActiveXControl`](../activexcontrol/).) |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Obtiene y establece el color ole del primer plano.(Hereda de [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Obtiene y establece la altura del control en unidades de puntos.(Hereda de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [HideSelection](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/hideselection/) { get; set; } | Indica si el texto seleccionado en el control aparece resaltado cuando el control no tiene el foco. |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | Obtiene y establece el modo de ejecución predeterminado del Editor de Métodos de Entrada para el control cuando recibe el foco.(Hereda de [`ActiveXControl`](../activexcontrol/).) |
| [IntegralHeight](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/integralheight/) { get; set; } | Indica si el control solo mostrará líneas completas de texto sin mostrar líneas parciales. |
| virtual [IsAutoSize](../../aspose.cells.drawing.activexcontrols/activexcontrol/isautosize/) { get; set; } | Indica si el control redimensionará automáticamente para mostrar todo su contenido.(Hereda de [`ActiveXControl`](../activexcontrol/).) |
| [IsAutoTab](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isautotab/) { get; set; } | Indica si el foco se moverá automáticamente al siguiente control cuando el usuario ingrese el número máximo de caracteres. |
| virtual [IsAutoWordSelected](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isautowordselected/) { get; set; } | Especifica la unidad básica utilizada para ampliar una selección. True indica que la unidad básica es un solo carácter. false indica que la unidad básica es una palabra completa. |
| [IsDragBehaviorEnabled](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/isdragbehaviorenabled/) { get; set; } | Indica si arrastrar y soltar está habilitado para el control. |
| [IsEditable](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/iseditable/) { get; set; } | Indica si el usuario puede escribir en el control. |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | Indica si el control puede recibir el foco y responder a eventos generados por el usuario.(Hereda de [`ActiveXControl`](../activexcontrol/).) |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | Indica si los datos del control están bloqueados para edición.(Hereda de [`ActiveXControl`](../activexcontrol/).) |
| [IsMultiLine](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/ismultiline/) { get; set; } | Indica si el control puede mostrar más de una línea de texto. |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | Indica si el control es transparente.(Heredado de [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Indica si este control es visible.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [IsWordWrapped](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/iswordwrapped/) { get; set; } | Indica si el contenido del control se ajusta automáticamente al final de una línea. |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Obtiene y establece la celda vinculada.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Obtiene y establece el rango de llenado de la lista.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MaxLength](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/maxlength/) { get; set; } | Obtiene y establece el número máximo de caracteres |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Obtiene y establece un ícono personalizado para mostrar como puntero del mouse del control.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Obtiene y establece el tipo de ícono que se muestra como puntero del mouse del control.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [PasswordChar](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/passwordchar/) { get; set; } | Obtiene y establece un carácter que se mostrará en lugar de los caracteres ingresados. |
| [ScrollBars](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/scrollbars/) { get; set; } | Indica si el control tiene barras de desplazamiento verticales, horizontales, ambas o ninguna. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Indica si se muestra una sombra.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ShowDropButtonTypeWhen](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/showdropbuttontypewhen/) { get; set; } | Especifica el símbolo mostrado en el botón desplegable |
| [SpecialEffect](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/specialeffect/) { get; set; } | Obtiene y establece el efecto especial del control. |
| [TabKeyBehavior](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/tabkeybehavior/) { get; set; } | Indica si se permiten caracteres de tabulación en el texto del control. |
| [Text](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/text/) { get; set; } | Obtiene y establece el texto del control. |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Representa cómo alinear el texto usado por el control.(Heredado de [`ActiveXControl`](../activexcontrol/).) |
| override [Type](../../aspose.cells.drawing.activexcontrols/textboxactivexcontrol/type/) { get; } | Obtiene el tipo del control ActiveX. |
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

    public class TextBoxActiveXControlDemo
    {
        public static void TextBoxActiveXControlExample()
        {
            // Inicializa un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar un TextBoxActiveXControl
            Shape shape = workbook.Worksheets[0].Shapes.AddActiveXControl(ControlType.TextBox, 1, 0, 1, 0, 100, 50);
            TextBoxActiveXControl activeXControl = (TextBoxActiveXControl)shape.ActiveXControl;

            // Estableciendo propiedades
            activeXControl.BorderStyle = ControlBorderType.Single;
            activeXControl.BorderOleColor = unchecked((int)0x80000012); // Excel default color system 12 or green(0x0000FF00)
            activeXControl.SpecialEffect = ControlSpecialEffectType.Bump;
            if (activeXControl.MaxLength == 0)
            {
                activeXControl.MaxLength = 30;
            }
            activeXControl.ScrollBars = ControlScrollBarType.BarsVertical;
            activeXControl.PasswordChar = 'a';
            if (!activeXControl.IsEditable)
            {
                activeXControl.IsEditable = true;
            }
            if (!activeXControl.IntegralHeight)
            {
                activeXControl.IntegralHeight = true;
            }
            if (!activeXControl.IsDragBehaviorEnabled)
            {
                activeXControl.IsDragBehaviorEnabled = true;
            }
            if (!activeXControl.EnterKeyBehavior)
            {
                activeXControl.EnterKeyBehavior = true;
            }
            if (!activeXControl.EnterFieldBehavior)
            {
                activeXControl.EnterFieldBehavior = true;
            }
            if (!activeXControl.TabKeyBehavior)
            {
                activeXControl.TabKeyBehavior = true;
            }
            if (!activeXControl.HideSelection)
            {
                activeXControl.HideSelection = true;
            }
            if (!activeXControl.IsAutoTab)
            {
                activeXControl.IsAutoTab = true;
            }
            if (!activeXControl.IsMultiLine)
            {
                activeXControl.IsMultiLine = true;
            }
            if (!activeXControl.IsAutoWordSelected)
            {
                activeXControl.IsAutoWordSelected = true;
            }
            if (!activeXControl.IsWordWrapped)
            {
                activeXControl.IsWordWrapped = true;
            }
            activeXControl.Text = "This is a test.";
            activeXControl.DropButtonStyle = DropButtonStyle.Arrow;
            activeXControl.ShowDropButtonTypeWhen = ShowDropButtonType.Focus;

            // Guarda el libro de trabajo
            workbook.Save("TextBoxActiveXControlExample.xlsx");
        }
    }
}
```

### Ver también

* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


