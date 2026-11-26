---
title: "ListBox.SelectedItem"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ListBox. Establece si el elemento está seleccionado"
type: docs
url: /es/net/aspose.cells.drawing/listbox/selecteditem/
---
## ListBox.SelectedItem method

Establece si el elemento está seleccionado

```csharp
public void SelectedItem(int itemIndex, bool isSelected)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| itemIndex | Int32 | El índice del elemento |
| isSelected | Booleano | Indica si el elemento está seleccionado. Verdadero significa que este elemento debe estar seleccionado. Falso significa que este elemento debe estar sin seleccionar. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ListBoxMethodSelectedItemWithInt32BooleanDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar elementos de la lista
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i, 0].Value = $"Item {i + 1}";
            }

            // Crear list box
            ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 1, 1, 150, 100) as ListBox;
            listBox.InputRange = "A1:A5";
            listBox.SelectionType = SelectionType.Multi;

            try
            {
                // Seleccionar y deseleccionar elementos
                listBox.SelectedItem(2, true);  // Select third item (index 2)
                listBox.SelectedItem(0, true);   // Select first item (index 0)
                listBox.SelectedItem(2, false); // Deselect third item

                // Verificar selecciones
                Console.WriteLine($"Item 0 selected: {listBox.IsSelected(0)}");
                Console.WriteLine($"Item 2 selected: {listBox.IsSelected(2)}");

                // Mostrar celdas seleccionadas
                Console.WriteLine("\nSelected Items:");
                foreach (Cell cell in listBox.SelectedCells)
                {
                    Console.WriteLine(cell.Value);
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }

            workbook.Save("ListBoxMethodSelectedItemWithInt32BooleanDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


