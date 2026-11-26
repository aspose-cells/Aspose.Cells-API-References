---
title: "ListBox.ItemCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListBox. Obtiene el número de elementos en el listbox"
type: docs
url: /es/net/aspose.cells.drawing/listbox/itemcount/
---
## ListBox.ItemCount property

Obtiene el número de elementos en el cuadro de lista.

```csharp
public int ItemCount { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ListBoxPropertyItemCountDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets.Add("Sheet1");

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Apple");
            worksheet.Cells["A2"].PutValue("Banana");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Mango");

            // Crear listbox y establecer propiedades
            Aspose.Cells.Drawing.ListBox listBox = worksheet.Shapes.AddListBox(1, 0, 10, 0, 100, 150);
            listBox.InputRange = "A1:A4";
            
            // Demostrar el uso de ItemCount
            int itemCount = listBox.ItemCount;
            Console.WriteLine("ListBox contains {0} items", itemCount);
            
            // Ajustar la altura del listbox según la cantidad de elementos
            listBox.Height = itemCount * 15;

            workbook.Save("ListBoxItemCountDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


