---
title: "ListBoxActiveXControl.ColumnWidths"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ListBoxActiveXControl propiedad. Obtiene y establece el ancho de la columna"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/columnwidths/
---
## ListBoxActiveXControl.ColumnWidths property

Obtiene y establece el ancho de la columna.

```csharp
public double ColumnWidths { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyColumnWidthsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 1, 100, 100);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            listBox.ColumnCount = 3;
            listBox.ColumnWidths = 50; // Changed from string to double
            
            worksheet.Cells["A2"].PutValue("Column1");
            worksheet.Cells["B2"].PutValue("Column2");
            worksheet.Cells["C2"].PutValue("Column3");
            worksheet.Cells["A3"].PutValue("Data1");
            worksheet.Cells["B3"].PutValue("Data2");
            worksheet.Cells["C3"].PutValue("Data3");
            
            listBox.ListFillRange = "A2:C3";

            workbook.Save("ListBoxColumnWidthsDemo.xlsx");
            Console.WriteLine("ListBox with custom column widths created successfully.");
        }
    }
}
```

### Ver también

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


