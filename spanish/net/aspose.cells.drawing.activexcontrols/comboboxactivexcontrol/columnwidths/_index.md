---
title: "ComboBoxActiveXControl.ColumnWidths"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ComboBoxActiveXControl. Obtiene y establece el ancho de la columna"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/columnwidths/
---
## ComboBoxActiveXControl.ColumnWidths property

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
    public class ComboBoxActiveXControlPropertyColumnWidthsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox,
                5, 0, 100, 20, 100, 20);
            
            var comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            comboBox.ColumnCount = 3;
            comboBox.ListRows = 5;
            
            // Establecer anchos de columna (usando un valor doble para el ancho de una sola columna)
            comboBox.ColumnWidths = 100;

            // Establecer elementos de lista mediante ListFillRange
            worksheet.Cells["A1"].PutValue("Product\tPrice\tStock");
            worksheet.Cells["A2"].PutValue("Laptop\t$999\t50");
            worksheet.Cells["A3"].PutValue("Phone\t$699\t120");
            worksheet.Cells["A4"].PutValue("Tablet\t$399\t75");
            comboBox.ListFillRange = "A1:A4";

            workbook.Save("ComboBoxColumnWidthsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


