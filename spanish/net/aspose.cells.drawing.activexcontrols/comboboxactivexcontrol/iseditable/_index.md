---
title: "ComboBoxActiveXControl.IsEditable"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ComboBoxActiveXControl. Indica si el usuario puede escribir en el control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/iseditable/
---
## ComboBoxActiveXControl.IsEditable property

Indica si el usuario puede escribir en el control.

```csharp
public bool IsEditable { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyIsEditableDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Acceder a la primera hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ComboBox usando la colección Shapes
            Shape shape = sheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 5, 0, 100, 30);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Establecer propiedades para el ComboBox
            comboBox.IsEditable = true;
            comboBox.Value = "Editable ComboBox";
            comboBox.ColumnCount = 2;
            comboBox.ListRows = 6;
            comboBox.TextColumn = 1;

            // Agregar elementos al ComboBox (usando la propiedad ListFillRange)
            sheet.Cells["A10"].PutValue("Item 1");
            sheet.Cells["B10"].PutValue("Description 1");
            sheet.Cells["A11"].PutValue("Item 2");
            sheet.Cells["B11"].PutValue("Description 2");
            comboBox.ListFillRange = "A10:B11";

            // Guarda el libro de trabajo
            workbook.Save("ComboBoxActiveXControl_IsEditableDemo.xlsx");

            // Verificar la propiedad después de guardar
            Console.WriteLine("IsEditable property value: " + comboBox.IsEditable);
        }
    }
}
```

### Ver también

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


