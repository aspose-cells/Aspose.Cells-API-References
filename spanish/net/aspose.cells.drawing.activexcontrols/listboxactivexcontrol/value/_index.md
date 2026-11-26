---
title: "ListBoxActiveXControl.Value"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListBoxActiveXControl. Obtiene y establece el valor del control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/value/
---
## ListBoxActiveXControl.Value property

Obtiene y establece el valor del control.

```csharp
public string Value { get; set; }
```

### Observaciones

Solo tiene efecto cuando [`SelectionType`](../selectiontype/) es SelectionType.Single;

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ListBox
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 1, 0, 1, 0, 100, 60);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)shape.ActiveXControl;

            // Establecer propiedades básicas
            listBox.ListWidth = 100;
            listBox.ColumnCount = 1;

            // Establezca los elementos usando la propiedad Value
            listBox.Value = "Red;Green;Blue;Yellow";

            // Guarda el libro de trabajo
            workbook.Save("ListBoxValueDemo.xlsx");

            Console.WriteLine("ListBox with items set using Value property has been created.");
        }
    }
}
```

### Ver también

* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


