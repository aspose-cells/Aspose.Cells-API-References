---
title: "ListBoxActiveXControl.ListStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ListBoxActiveXControl. Obtiene y establece la apariencia visual"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/listboxactivexcontrol/liststyle/
---
## ListBoxActiveXControl.ListStyle property

Obtiene y establece la apariencia visual.

```csharp
public ControlListStyle ListStyle { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ListBoxActiveXControlPropertyListStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para el list box
            sheet.Cells["A3"].Value = "Sales";
            sheet.Cells["A4"].Value = "Finance";
            sheet.Cells["A5"].Value = "MIS";
            sheet.Cells["A6"].Value = "R&D";
            sheet.Cells["A7"].Value = "Marketing";

            // Agregar un control ActiveX ListBox
            Shape shape = sheet.Shapes.AddActiveXControl(ControlType.ListBox, 5, 0, 5, 0, 100, 200);
            ListBoxActiveXControl listBox = (ListBoxActiveXControl)shape.ActiveXControl;

            // Configure las propiedades del ListBox
            listBox.ListFillRange = "A3:A7";
            listBox.LinkedCell = "B1";
            listBox.ListStyle = ControlListStyle.Option; // Demonstrating ListStyle property
            listBox.SelectionType = SelectionType.Single;

            // Guarda el libro de trabajo
            workbook.Save("ListBoxActiveXControl_ListStyle_Demo.xlsx");
        }
    }
}
```

### Ver también

* enum [ControlListStyle](../../controlliststyle/)
* class [ListBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


