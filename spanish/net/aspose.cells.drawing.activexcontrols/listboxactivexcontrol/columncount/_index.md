---
title: "ListBoxActiveXControl.ColumnCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListBoxActiveXControl. Representa el número de columnas a mostrar en un ComboBox o ListBox"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/columncount/
---
## ListBoxActiveXControl.ColumnCount property

Representa el número de columnas a mostrar en un ComboBox o ListBox.

```csharp
public int ColumnCount { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyColumnCountDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ListBox
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 1, 1, 1, 1, 200, 100);
            var listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Establezca propiedades incluyendo ColumnCount
            listBox.ColumnCount = 3;
            listBox.ListFillRange = "A1:C3"; // Sample data range for 3 columns

            // Verifique y muestre el ColumnCount
            Console.WriteLine("ListBox ColumnCount: " + listBox.ColumnCount);

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


