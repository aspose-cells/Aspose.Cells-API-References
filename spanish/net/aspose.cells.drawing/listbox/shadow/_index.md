---
title: "ListBox.Shadow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListBox. Indica si el combobox tiene sombreado 3D"
type: docs
url: /es/net/aspose.cells.drawing/listbox/shadow/
---
## ListBox.Shadow property

Indica si el cuadro combinado tiene sombreado 3D.

```csharp
public bool Shadow { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertyShadowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Poblar elementos de la lista
            worksheet.Cells["A1"].PutValue("Option 1");
            worksheet.Cells["A2"].PutValue("Option 2");
            worksheet.Cells["A3"].PutValue("Option 3");

            // Crear listbox y establecer propiedades principales
            ListBox listBox = worksheet.Shapes.AddListBox(2, 1, 5, 1, 100, 150);
            listBox.InputRange = "A1:A3";
            listBox.LinkedCell = "B1";
            
            // Establecer la propiedad shadow
            listBox.Shadow = true;

            // Guarde y recargue para verificar
            workbook.Save("ListBoxShadowDemo.xlsx");
            
            Workbook loadedWorkbook = new Workbook("ListBoxShadowDemo.xlsx");
            ListBox loadedBox = (ListBox)loadedWorkbook.Worksheets[0].Shapes[0];
            
            Console.WriteLine("Shadow enabled: " + loadedBox.Shadow);
        }
    }
}
```

### Ver también

* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


