---
title: "ListBox.SelectedIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListBox. Obtiene o establece el número de índice del elemento actualmente seleccionado en un list box o combo box. Basado en cero"
type: docs
url: /es/net/aspose.cells.drawing/listbox/selectedindex/
---
## ListBox.SelectedIndex property

Obtiene o establece el número de índice del elemento actualmente seleccionado en un cuadro de lista o cuadro combinado. Basado en cero.

```csharp
public int SelectedIndex { get; set; }
```

### Observaciones

-1 presents no item is selected.

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertySelectedIndexDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["A1"].PutValue("Item 0");
            worksheet.Cells["A2"].PutValue("Item 1");
            worksheet.Cells["A3"].PutValue("Item 2");
            
            ListBox listBox = worksheet.Shapes.AddListBox(5, 5, 100, 100, 200, 300);
            listBox.InputRange = "A1:A3";
            listBox.LinkedCell = "B1";
            
            listBox.SelectedIndex = 2;
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


