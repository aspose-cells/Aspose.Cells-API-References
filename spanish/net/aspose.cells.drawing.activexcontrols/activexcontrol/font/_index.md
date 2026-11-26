---
title: "ActiveXControl.Font"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ActiveXControl. Representa la fuente del control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/activexcontrol/font/
---
## ActiveXControl.Font property

Representa la fuente del control.

```csharp
public Font Font { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using Aspose.Cells.Drawing.ActiveXControls;
    using System;

    public class ActiveXControlPropertyFontDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar un control ActiveX (Label) a la hoja de cálculo
                Shape shape = worksheet.Shapes.AddActiveXControl(
                    ControlType.Label,
                    1, 1, 200, 50,
                    0, 0);

                // Obtener la instancia del control ActiveX
                LabelActiveXControl label = (LabelActiveXControl)shape.ActiveXControl;

                // Establecer algunas propiedades básicas
                label.Caption = "Sample Label";

                // Acceder a la propiedad Font (solo lectura)
                Font controlFont = label.Font;

                // Mostrar propiedades de la fuente
                Console.WriteLine("Font Name: " + controlFont.Name);
                Console.WriteLine("Font Size: " + controlFont.Size);
                Console.WriteLine("Is Bold: " + controlFont.IsBold);
                Console.WriteLine("Is Italic: " + controlFont.IsItalic);
                Console.WriteLine("Color: " + controlFont.Color);
                Console.WriteLine("Underline Type: " + controlFont.Underline);

                // Guarda el libro de trabajo
                workbook.Save("FontDemo.xlsx");
                Console.WriteLine("Font properties demonstrated successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [Font](../../../aspose.cells/font/)
* class [ActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


