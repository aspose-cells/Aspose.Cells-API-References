---
title: "ComboBoxActiveXControl.Value"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ComboBoxActiveXControl. Obtiene y establece el valor del control"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/value/
---
## ComboBoxActiveXControl.Value property

Obtiene y establece el valor del control.

```csharp
public string Value { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ComboBox a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 1, 1, 0, 0, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Establecer propiedades para el ComboBox
            comboBox.Value = "Initial Value";
            comboBox.ListFillRange = "A1:A3";
            
            // Agregar algunos datos de muestra al rango de lista
            worksheet.Cells["A1"].PutValue("Option 1");
            worksheet.Cells["A2"].PutValue("Option 2");
            worksheet.Cells["A3"].PutValue("Option 3");

            // Actualizar el valor seleccionado desde la celda vinculada
            worksheet.Cells["B1"].PutValue("Option 2");
            worksheet.Shapes.UpdateSelectedValue();

            // Demostrar la obtención de la propiedad Value
            Console.WriteLine("ComboBox Value: " + comboBox.Value);

            // Guarda el libro de trabajo
            workbook.Save("ComboBoxActiveXControlDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


