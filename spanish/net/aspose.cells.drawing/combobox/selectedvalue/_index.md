---
title: "ComboBox.SelectedValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ComboBox. Obtiene el valor seleccionado del cuadro combinado"
type: docs
url: /es/net/aspose.cells.drawing/combobox/selectedvalue/
---
## ComboBox.SelectedValue property

Obtiene el valor seleccionado del cuadro combinado.

```csharp
public string SelectedValue { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxPropertySelectedValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un ComboBox y agregar elementos
            Aspose.Cells.Drawing.ComboBox comboBox = (Aspose.Cells.Drawing.ComboBox)worksheet.Shapes.AddComboBox(1, 0, 1, 0, 100, 50);
            comboBox.LinkedCell = "A1";
            comboBox.SetInputRange("B1:B4", false, false);
            
            // Establecer valores en el rango de entrada
            worksheet.Cells["B1"].PutValue("a");
            worksheet.Cells["B2"].PutValue("b");
            worksheet.Cells["B3"].PutValue("c");
            worksheet.Cells["B4"].PutValue("d");

            // Demostrar SelectedValue (propiedad de solo lectura)
            Console.WriteLine("SelectedValue: " + comboBox.SelectedValue);

            // Guarda el libro de trabajo
            workbook.Save("ComboBoxDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


