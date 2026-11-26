---
title: "ListBox.PageChange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListBox. Especifica la cantidad en que el valor del control cambia cuando el usuario hace clic en la zona de página arriba o página abajo de las barras de desplazamiento"
type: docs
url: /es/net/aspose.cells.drawing/listbox/pagechange/
---
## ListBox.PageChange property

Especifica la cantidad en que se cambia el valor del control cuando el usuario hace clic en la zona de subir o bajar página de la barra de desplazamiento.

```csharp
public int PageChange { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertyPageChangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma ListBox
            ListBox listBox = (ListBox)worksheet.Shapes.AddListBox(1, 0, 1, 0, 100, 100);

            // Establecer algunos elementos para el ListBox
            listBox.SetInputRange("A1:A5", false, false);
            
            // Establecer la propiedad PageChange
            listBox.PageChange = 2;

            // Guarda el libro de trabajo
            workbook.Save("ListBoxPageChangeDemo.xlsx");

            // Mostrar el valor de PageChange
            Console.WriteLine("ListBox PageChange value: " + listBox.PageChange);
        }
    }
}
```

### Ver también

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


