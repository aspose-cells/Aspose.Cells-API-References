---
title: "LabelActiveXControl.Picture"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LabelActiveXControl. Obtiene y establece los datos de la imagen"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/labelactivexcontrol/picture/
---
## LabelActiveXControl.Picture property

Obtiene y establece los datos de la imagen.

```csharp
public byte[] Picture { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.IO;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class LabelActiveXControlPropertyPictureDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX Label
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.Label, 1, 1, 1, 1, 100, 50);
            LabelActiveXControl labelControl = (LabelActiveXControl)shape.ActiveXControl;

            // Establecer propiedades básicas
            labelControl.Caption = "Sample Label";
            labelControl.PicturePosition = ControlPicturePositionType.LeftTop;

            // Cargar una imagen para la propiedad Picture
            string imagePath = "sample.jpg"; // Replace with actual image path
            if (File.Exists(imagePath))
            {
                labelControl.Picture = File.ReadAllBytes(imagePath);
                Console.WriteLine("Picture set successfully");
            }
            else
            {
                Console.WriteLine("Image file not found, using null picture");
                labelControl.Picture = null;
            }

            // Guarda el libro de trabajo
            workbook.Save("LabelActiveXControlDemo.xlsx");
        }
    }
}
```

### Ver también

* class [LabelActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


