---
title: "ListBoxActiveXControl.ShowColumnHeads"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "ListBoxActiveXControl propiedad. Indica si se muestran los encabezados de columna"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/showcolumnheads/
---
## ListBoxActiveXControl.ShowColumnHeads property

Indica si se muestran los encabezados de columna.

```csharp
public bool ShowColumnHeads { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyShowColumnHeadsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agrega un control ListBox ActiveX con todos los parámetros requeridos
            Shape shape = worksheet.Shapes.AddActiveXControl(
                ControlType.ListBox, 
                1, 1, 100, 100,  // Left, Top, Width, Height
                0, 0);           // UpperLeftRow, UpperLeftColumn

            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Establecer propiedades para el ListBox
            listBox.ColumnCount = 2;
            listBox.ListWidth = 150;
            listBox.ShowColumnHeads = true; // Demonstrate ShowColumnHeads property

            // Agregar algunos datos de ejemplo
            listBox.Value = "Header1\tHeader2\nItem1\tData1\nItem2\tData2";

            // Guarda el libro de trabajo
            workbook.Save("ListBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


