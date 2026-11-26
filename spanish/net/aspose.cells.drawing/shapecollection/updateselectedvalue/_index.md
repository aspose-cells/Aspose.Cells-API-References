---
title: "ShapeCollection.UpdateSelectedValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Actualiza el valor seleccionado con el valor de la celda vinculada o del rango de la forma"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/updateselectedvalue/
---
## ShapeCollection.UpdateSelectedValue method

Actualiza el valor seleccionado con el valor de la celda vinculada o del rango de la forma.

```csharp
public void UpdateSelectedValue()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodUpdateSelectedValueDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Añade una forma (lista desplegable) a la hoja de cálculo
            Aspose.Cells.Drawing.ListBox listBox = (Aspose.Cells.Drawing.ListBox)worksheet.Shapes.AddListBox(0, 0, 100, 100, 3, 20);
            
            // Establece los elementos de la lista y el valor seleccionado
            listBox.SetInputRange("A1:A3", false, false);
            listBox.SelectedIndex = 1;
            
            // Actualiza el valor seleccionado en la forma
            worksheet.Shapes.UpdateSelectedValue();
            
            // Guarda el libro de trabajo
            workbook.Save("ShapeCollectionUpdateSelectedValueDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


