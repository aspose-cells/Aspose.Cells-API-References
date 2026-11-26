---
title: "ComboBox.SelectedCell"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de ComboBox. Obtiene la celda seleccionada en el rango de entrada del combo box"
type: docs
url: /es/net/aspose.cells.drawing/combobox/selectedcell/
---
## ComboBox.SelectedCell property

Obtiene la celda seleccionada en el rango de entrada del cuadro combinado.

```csharp
public Cell SelectedCell { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ComboBoxPropertySelectedCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar celdas con datos de ejemplo para los elementos del combobox
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Cherry");
            worksheet.Cells["A4"].PutValue("Date");
            worksheet.Cells["A5"].PutValue("Fig");

            // Crear un ComboBox y establecer sus propiedades
            ComboBox comboBox = worksheet.Shapes.AddComboBox(0, 0, 100, 100, 5, 0);
            comboBox.InputRange = "A1:A5";
            comboBox.DropDownLines = 5;

            // Establecer la selección y demostrar SelectedCell
            comboBox.SelectedIndex = 2;
            Cell selectedCell = comboBox.SelectedCell;

            Console.WriteLine($"Initial Selected Cell Value: {selectedCell.StringValue}");

            // Modificar el valor de la celda seleccionada
            selectedCell.PutValue("Orange");
            Console.WriteLine($"Updated Selected Cell Value: {selectedCell.StringValue}");

            // Mostrar el efecto en las celdas adyacentes
            worksheet.Cells["B3"].PutValue($"Combo Selection: {comboBox.SelectedValue}");

            workbook.Save("ComboBoxSelectedCellDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../../../aspose.cells/cell/)
* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


