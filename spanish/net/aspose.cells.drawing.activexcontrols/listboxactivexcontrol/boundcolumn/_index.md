---
title: "ListBoxActiveXControl.BoundColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListBoxActiveXControl. Representa cómo se determina la propiedad Value para un ComboBox o ListBox cuando el valor de la propiedad MultiSelect es fmMultiSelectSingle"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/boundcolumn/
---
## ListBoxActiveXControl.BoundColumn property

Representa cómo se determina la propiedad Value para un ComboBox o ListBox cuando el valor de la propiedad MultiSelect es (fmMultiSelectSingle).

```csharp
public int BoundColumn { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyBoundColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["B2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["B3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B4"].PutValue("Banana");

            // Agrega un control ListBox ActiveX
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 0, 150, 100);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Configura las propiedades del ListBox
            listBox.ColumnCount = 2;
            listBox.ListFillRange = "A1:B4";
            
            // Establezca BoundColumn a 0 (columna ID) - este será el valor devuelto cuando se seleccione un elemento
            listBox.BoundColumn = 0;
            
            // Establezca TextColumn a 1 (columna Nombre) - esto se mostrará en la lista
            listBox.TextColumn = 1;

            // Guarda el libro de trabajo
            workbook.Save("ListBoxBoundColumnDemo.xlsx");

            Console.WriteLine("ListBox BoundColumn set to: " + listBox.BoundColumn);
        }
    }
}
```

### Ver también

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


