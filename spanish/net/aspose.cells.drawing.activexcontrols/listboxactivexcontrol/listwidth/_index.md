---
title: "ListBoxActiveXControl.ListWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListBoxActiveXControl. Obtiene y establece el ancho en unidades de puntos"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/listwidth/
---
## ListBoxActiveXControl.ListWidth property

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
    public class ListBoxActiveXControlPropertyListWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue un control ListBox ActiveX con todos los parámetros requeridos
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 
                10, 10, 200, 100, 200, 100);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Establezca la propiedad ListWidth
            listBox.ListWidth = 150;
            
            // Configurar propiedades básicas
            listBox.ColumnCount = 2;
            listBox.ColumnWidths = 100; // Changed from string to double
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["B1"].PutValue("Red");
            worksheet.Cells["B2"].PutValue("Yellow");
            worksheet.Cells["B3"].PutValue("Orange");
            
            // Establecer rango de datos
            listBox.ListFillRange = "A1:B3";

            workbook.Save("ListBoxWidthDemo.xlsx");
            Console.WriteLine("ListBox with ListWidth=150 created successfully.");
        }
    }
}
```

### Ver también

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


