---
title: "CommandButtonActiveXControl.Picture"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CommandButtonActiveXControl. Obtiene y establece los datos de la imagen"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/commandbuttonactivexcontrol/picture/
---
## CommandButtonActiveXControl.Picture property

Obtiene y establece los datos de la imagen.

```csharp
public byte[] Picture { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class CommandButtonActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear una forma para alojar el control ActiveX con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.CommandButton, 
                1,  // top row
                1,  // left column
                0,  // top position
                0,  // left position
                100, // width
                30); // height
                
            CommandButtonActiveXControl button = (CommandButtonActiveXControl)shape.ActiveXControl;

            // Establecer propiedades
            button.Caption = "Click Me";
            button.PicturePosition = ControlPicturePositionType.AboveCenter;

            // Establece la imagen (un arreglo de bytes vacío representa ninguna imagen)
            button.Picture = new byte[0];

            // Guarda el libro de trabajo
            workbook.Save("CommandButtonWithPicture.xlsx");

            // Verifica la propiedad Picture
            Console.WriteLine("Picture is null: " + (button.Picture == null));
        }
    }
}
```

### Ver también

* class [CommandButtonActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


