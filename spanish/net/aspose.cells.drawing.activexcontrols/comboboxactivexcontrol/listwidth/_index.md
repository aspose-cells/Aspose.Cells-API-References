---
title: "ComboBoxActiveXControl.ListWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ComboBoxActiveXControl. Obtiene y establece el ancho en unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/listwidth/
---
## ComboBoxActiveXControl.ListWidth property

Obtiene y establece el ancho en unidades de puntos.

```csharp
public double ListWidth { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyListWidthDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el ComboBox
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");

            // Agregar un control ActiveX ComboBox con todos los parámetros requeridos
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox,
                1,  // left
                1,  // top
                100, // width
                30,  // height
                0,   // image width (unused for ComboBox)
                0    // image height (unused for ComboBox)
            );
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Establecer la propiedad ListWidth para controlar el ancho del desplegable
            comboBox.ListWidth = 150;
            comboBox.ListRows = 3;
            comboBox.LinkedCell = "A1:A3";

            // Guarda el libro de trabajo
            workbook.Save("ComboBoxListWidthDemo.xlsx");

            Console.WriteLine("ComboBox ListWidth set to: " + comboBox.ListWidth);
        }
    }
}
```

### Ver también

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


