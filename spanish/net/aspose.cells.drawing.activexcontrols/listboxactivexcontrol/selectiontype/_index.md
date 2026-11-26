---
title: "ListBoxActiveXControl.SelectionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListBoxActiveXControl. Indica si el control permite selecciones múltiples"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/selectiontype/
---
## ListBoxActiveXControl.SelectionType property

Indica si el control permite selecciones múltiples.

```csharp
public SelectionType SelectionType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertySelectionTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Agrega un control ListBox ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 0, 100, 60);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Configura las propiedades del ListBox
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;
            
            // Demostrar la propiedad SelectionType
            listBox.SelectionType = SelectionType.Single; // Only single selection allowed
            listBox.Value = "Apple;Banana;Cherry";

            // Guarda el libro de trabajo
            workbook.Save("ListBoxSelectionTypeDemo.xlsx");

            Console.WriteLine("ListBox with Single SelectionType created successfully.");
        }
    }
}
```

### Ver también

* enum [SelectionType](../../../aspose.cells.drawing/selectiontype/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


