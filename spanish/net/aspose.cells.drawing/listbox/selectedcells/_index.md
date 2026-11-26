---
title: "ListBox.SelectedCells"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListBox. Obtiene las celdas seleccionadas. Devuelve null si el rango de entrada no está establecido o no hay ningún elemento seleccionado"
type: docs
url: /es/net/aspose.cells.drawing/listbox/selectedcells/
---
## ListBox.SelectedCells property

Obtiene las celdas seleccionadas. Devuelve null si el rango de entrada no está configurado o no se ha seleccionado ningún elemento

```csharp
public Cell[] SelectedCells { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ListBoxPropertySelectedCellsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar datos de ejemplo para los elementos del ListBox
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");

            // Crear un ListBox y enlazarlo al rango de datos
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(7, 0, 100, 150, 5, 1);
            listBox.InputRange = "A1:A5";
            listBox.SelectionType = SelectionType.Multi;

            // Seleccionar varios elementos usando índices basados en cero
            listBox.SelectedItem(0, true);
            listBox.SelectedItem(2, true);

            // Recuperar y mostrar las celdas seleccionadas
            Cell[] selectedCells = listBox.SelectedCells;
            Console.WriteLine("Selected Cells Count: " + selectedCells.Length);
            
            // Modificar las celdas seleccionadas para demostrar el acceso
            foreach (Cell cell in selectedCells)
            {
                Console.WriteLine("Selected Cell Address: " + cell.Name);
                cell.PutValue("[SELECTED] " + cell.StringValue);
            }

            workbook.Save("ListBoxSelectedCellsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Cell](../../../aspose.cells/cell/)
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


