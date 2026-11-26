---
title: "Clase ImageActiveXControl"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Drawing.ActiveXControls.ImageActiveXControl. Representa el control de imagen"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/imageactivexcontrol/
---
## ImageActiveXControl class

Representa el control de imagen.

```csharp
public class ImageActiveXControl : ActiveXControl
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| virtual [BackOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/backolecolor/) { get; set; } | Obtiene y establece el color ole del fondo.(Hereda de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [BorderOleColor](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/borderolecolor/) { get; set; } | Obtiene y establece el color ole del fondo. |
| [BorderStyle](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/borderstyle/) { get; set; } | Obtiene y establece el tipo de borde utilizado por el control. |
| override [Data](../../aspose.cells.drawing.activexcontrols/activexcontrol/data/) { get; } | Obtiene y establece los datos binarios del control.(Hereda de [`ActiveXControl`](../activexcontrol/).) |
| [Font](../../aspose.cells.drawing.activexcontrols/activexcontrol/font/) { get; } | Representa la fuente del control.(Hereda de [`ActiveXControl`](../activexcontrol/).) |
| virtual [ForeOleColor](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/foreolecolor/) { get; set; } | Obtiene y establece el color ole del primer plano.(Hereda de [`ActiveXControlBase`](../activexcontrolbase/).) |
| virtual [Height](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/height/) { get; set; } | Obtiene y establece la altura del control en unidades de puntos.(Hereda de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [IMEMode](../../aspose.cells.drawing.activexcontrols/activexcontrol/imemode/) { get; set; } | Obtiene y establece el modo de ejecución predeterminado del Editor de Métodos de Entrada para el control cuando recibe el foco.(Hereda de [`ActiveXControl`](../activexcontrol/).) |
| override [IsAutoSize](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/isautosize/) { get; set; } | Indica si el control cambiará de tamaño automáticamente para mostrar todo su contenido. |
| [IsEnabled](../../aspose.cells.drawing.activexcontrols/activexcontrol/isenabled/) { get; set; } | Indica si el control puede recibir el foco y responder a eventos generados por el usuario.(Hereda de [`ActiveXControl`](../activexcontrol/).) |
| [IsLocked](../../aspose.cells.drawing.activexcontrols/activexcontrol/islocked/) { get; set; } | Indica si los datos del control están bloqueados para edición.(Hereda de [`ActiveXControl`](../activexcontrol/).) |
| [IsTiled](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/istiled/) { get; set; } | Indica si la imagen se repite en forma de mosaico en el fondo. |
| [IsTransparent](../../aspose.cells.drawing.activexcontrols/activexcontrol/istransparent/) { get; set; } | Indica si el control es transparente.(Heredado de [`ActiveXControl`](../activexcontrol/).) |
| virtual [IsVisible](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/isvisible/) { get; set; } | Indica si este control es visible.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [LinkedCell](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/linkedcell/) { get; set; } | Obtiene y establece la celda vinculada.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [ListFillRange](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/listfillrange/) { get; set; } | Obtiene y establece el rango de llenado de la lista.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MouseIcon](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mouseicon/) { get; set; } | Obtiene y establece un ícono personalizado para mostrar como puntero del mouse del control.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [MousePointer](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/mousepointer/) { get; set; } | Obtiene y establece el tipo de ícono que se muestra como puntero del mouse del control.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Picture](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/picture/) { get; set; } | Obtiene y establece los datos de la imagen. |
| [PictureAlignment](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/picturealignment/) { get; set; } | Obtiene y establece la alineación de la imagen dentro del Formulario o Imagen. |
| [PictureSizeMode](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/picturesizemode/) { get; set; } | Obtiene y establece cómo mostrar la imagen. |
| virtual [Shadow](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/shadow/) { get; set; } | Indica si se muestra una sombra.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [SpecialEffect](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/specialeffect/) { get; set; } | Obtiene y establece el efecto especial del control. |
| [TextAlign](../../aspose.cells.drawing.activexcontrols/activexcontrol/textalign/) { get; set; } | Representa cómo alinear el texto usado por el control.(Heredado de [`ActiveXControl`](../activexcontrol/).) |
| override [Type](../../aspose.cells.drawing.activexcontrols/imageactivexcontrol/type/) { get; } | Obtiene el tipo del control ActiveX. |
| virtual [Width](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/width/) { get; set; } | Obtiene y establece el ancho del control en unidades de puntos.(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |
| [Workbook](../../aspose.cells.drawing.activexcontrols/activexcontrolbase/workbook/) { get; } | Obtiene el objeto [`Workbook`](../activexcontrolbase/workbook/).(Heredado de [`ActiveXControlBase`](../activexcontrolbase/).) |

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;
using System;
using System.IO;

namespace AsposeCellsExamples
{
    public class ImageActiveXControlDemo
    {
        public static void RunDemo()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control Image ActiveX a la hoja de cálculo
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.Image, 5, 0, 1, 1, 100, 100);
            ImageActiveXControl imageControl = (ImageActiveXControl)shape.ActiveXControl;

            // Establecer propiedades para el control Image ActiveX
            imageControl.IsAutoSize = true;
            imageControl.BorderOleColor = 0x000000; // Black border
            imageControl.BorderStyle = ControlBorderType.Single;
            imageControl.PictureSizeMode = ControlPictureSizeMode.Stretch;
            imageControl.SpecialEffect = ControlSpecialEffectType.Flat;
            imageControl.PictureAlignment = ControlPictureAlignmentType.Center;
            imageControl.IsTiled = false;

            // Cargar una imagen desde un archivo y asignarla al control
            byte[] imageData = File.ReadAllBytes("ImageActiveXControlDemo.jpg");
            imageControl.Picture = imageData;

            // Guarda el libro de trabajo
            workbook.Save("ImageActiveXControlDemo.xlsx");
            workbook.Save("ImageActiveXControlDemo.pdf");

            // Genere la salida de los resultados
            Console.WriteLine("Image ActiveX Control added with the following properties:");
            Console.WriteLine($"IsAutoSize: {imageControl.IsAutoSize}");
            Console.WriteLine($"BorderOleColor: {imageControl.BorderOleColor}");
            Console.WriteLine($"BorderStyle: {imageControl.BorderStyle}");
            Console.WriteLine($"PictureSizeMode: {imageControl.PictureSizeMode}");
            Console.WriteLine($"SpecialEffect: {imageControl.SpecialEffect}");
            Console.WriteLine($"PictureAlignment: {imageControl.PictureAlignment}");
            Console.WriteLine($"IsTiled: {imageControl.IsTiled}");
        }
    }
}
```

### Ver también

* class [ActiveXControl](../activexcontrol/)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../)


