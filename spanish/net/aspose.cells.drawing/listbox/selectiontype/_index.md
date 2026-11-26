---
title: "ListBox.SelectionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListBox. Obtiene o establece el modo de selección del list box especificado"
type: docs
url: /es/net/aspose.cells.drawing/listbox/selectiontype/
---
## ListBox.SelectionType property

Obtiene o establece el modo de selección del cuadro de lista especificado.

```csharp
public SelectionType SelectionType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ListBoxPropertySelectionTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo Workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para el list box
            sheet.Cells["A1"].PutValue("Sales");
            sheet.Cells["A2"].PutValue("Finance");
            sheet.Cells["A3"].PutValue("MIS");
            sheet.Cells["A4"].PutValue("R&D");

            // Agregar un list box
            ListBox listBox = sheet.Shapes.AddListBox(1, 0, 2, 0, 100, 80);
            
            // Establecer propiedades del list box
            listBox.InputRange = "A1:A4";
            listBox.LinkedCell = "B1";
            
            // Demostrar la propiedad SelectionType
            listBox.SelectionType = SelectionType.Single; // Only single selection allowed
            listBox.SelectedIndex = 1; // Select "Finance"

            // Guarda el libro de trabajo
            workbook.Save("ListBoxSelectionTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [SelectionType](../../selectiontype/)
* class [ListBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


