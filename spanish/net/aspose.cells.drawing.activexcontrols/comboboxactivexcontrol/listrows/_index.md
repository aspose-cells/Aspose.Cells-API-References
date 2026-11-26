---
title: "ComboBoxActiveXControl.ListRows"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ComboBoxActiveXControl. Representa el número máximo de filas a mostrar en la lista"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/listrows/
---
## ComboBoxActiveXControl.ListRows property

Representa el número máximo de filas a mostrar en la lista.

```csharp
public int ListRows { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyListRowsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ComboBox ActiveX con los parámetros de ancho/alto adecuados
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 10, 10, 150, 30, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Agregar elementos de muestra al cuadro combinado usando ListFillRange
            comboBox.ListFillRange = "A1:A7";
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");
            worksheet.Cells["A6"].PutValue("Item 6");
            worksheet.Cells["A7"].PutValue("Item 7");

            // Establecer la propiedad ListRows para controlar los elementos visibles en el desplegable
            comboBox.ListRows = 4; // Only show 4 items at a time

            // Guarda el libro de trabajo
            workbook.Save("ComboBoxListRowsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


