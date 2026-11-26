---
title: "Shape.UpdateSelectedValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Shape. Actualiza el valor seleccionado por el valor de la celda vinculada"
type: docs
url: /es/net/aspose.cells.drawing/shape/updateselectedvalue/
---
## Shape.UpdateSelectedValue method

Actualiza el valor seleccionado con el valor de la celda vinculada.

```csharp
public void UpdateSelectedValue()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeMethodUpdateSelectedValueDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar algunos datos de muestra
            for (int i = 0; i < 10; i++)
            {
                worksheet.Cells[i, 0].Value = i + 1;
            }

            // Crear una forma ListBox
            Shape listBoxShape = worksheet.Shapes.AddListBox(2, 0, 2, 0, 130, 130);
            
            // Establecer rango de entrada y celda vinculada
            listBoxShape.SetInputRange("$A$1:$A$6", false, false);
            listBoxShape.SetLinkedCell("$A$12", false, true);

            // Obtener el objeto ListBox
            ListBox listBox = (ListBox)listBoxShape;

            // Establecer el valor inicial en la celda vinculada y actualizar la selección
            worksheet.Cells["A12"].Value = 3;
            listBoxShape.UpdateSelectedValue();

            // Verificar la selección
            if (listBox.IsSelected(2))
            {
                Console.WriteLine("Option 3 is selected");
            }

            // Cambiar el valor y actualizar la selección nuevamente
            worksheet.Cells["A12"].Value = 4;
            listBoxShape.UpdateSelectedValue();

            if (listBox.IsSelected(3))
            {
                Console.WriteLine("Option 4 is selected");
            }
        }
    }
}
```

### Ver también

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


