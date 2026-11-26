---
title: "ComboBox.SelectedIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ComboBox. Obtiene o establece el número de índice del elemento seleccionado actualmente en una lista o cuadro combinado. Basado en cero"
type: docs
url: /es/net/aspose.cells.drawing/combobox/selectedindex/
---
## ComboBox.SelectedIndex property

Obtiene o establece el número de índice del elemento actualmente seleccionado en un cuadro de lista o cuadro combinado. Basado en cero.

```csharp
public int SelectedIndex { get; set; }
```

### Observaciones

-1 presents no item is selected.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxPropertySelectedIndexDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el cuadro combinado
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");

            // Agregar un cuadro combinado a la hoja de cálculo
            Shape shape = worksheet.Shapes.AddComboBox(1, 0, 1, 0, 100, 20);
            ComboBox comboBox = (ComboBox)shape;

            // Establecer el rango de entrada para el cuadro combinado
            comboBox.InputRange = "A1:A5";
            comboBox.DropDownLines = 5;

            // Establecer y mostrar el índice seleccionado
            comboBox.SelectedIndex = 2; // Selects "Item 3" (zero-based index)
            Console.WriteLine("Selected Index: " + comboBox.SelectedIndex);
            Console.WriteLine("Selected Value: " + comboBox.SelectedValue);

            // Cambiar el índice seleccionado y mostrarlo nuevamente
            comboBox.SelectedIndex = 4; // Selects "Item 5"
            Console.WriteLine("\nAfter changing selection:");
            Console.WriteLine("Selected Index: " + comboBox.SelectedIndex);
            Console.WriteLine("Selected Value: " + comboBox.SelectedValue);
        }
    }
}
```

### Ver también

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


