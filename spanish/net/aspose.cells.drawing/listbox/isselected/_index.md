---
title: "ListBox.IsSelected"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ListBox. Indica si el elemento está seleccionado"
type: docs
url: /es/net/aspose.cells.drawing/listbox/isselected/
---
## ListBox.IsSelected method

Indica si el elemento está seleccionado.

```csharp
public bool IsSelected(int itemIndex)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| itemIndex | Int32 | El índice del elemento. |

### Valor de retorno

si el elemento está seleccionado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxMethodIsSelectedWithInt32Demo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un cuadro de lista a la hoja de cálculo
            ListBox listBox = worksheet.Shapes.AddListBox(0, 0, 100, 100, 200, 200);

            // Establecer los elementos de la lista a través del rango de celdas vinculado
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            listBox.LinkedCell = "A1:A3";

            // Selecciona un elemento
            listBox.SelectedIndex = 0;

            // Verifica el estado de selección usando IsSelected con un parámetro Int32
            Console.WriteLine("Item 0 selected: " + listBox.IsSelected(0));
            Console.WriteLine("Item 1 selected: " + listBox.IsSelected(1));
            Console.WriteLine("Item 2 selected: " + listBox.IsSelected(2));
        }
    }
}
```

### Ver también

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


