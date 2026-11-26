---
title: "ComboBoxActiveXControl.ListStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ComboBoxActiveXControl. Obtiene y establece la apariencia visual"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/liststyle/
---
## ComboBoxActiveXControl.ListStyle property

Obtiene y establece la apariencia visual.

```csharp
public ControlListStyle ListStyle { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyListStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Items");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Orange");

            // Agregar ComboBox con estilo de lista simple
            var comboBoxShape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 1, 0, 1, 0, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)comboBoxShape.ActiveXControl;
            comboBox.ListStyle = Aspose.Cells.Drawing.ActiveXControls.ControlListStyle.Plain;
            comboBox.ListFillRange = "A2:A4";

            // Agregar ListBox con estilo de lista de opciones
            var listBoxShape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox, 5, 0, 1, 0, 100, 60);
            Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl listBox = (Aspose.Cells.Drawing.ActiveXControls.ListBoxActiveXControl)listBoxShape.ActiveXControl;
            listBox.ListStyle = Aspose.Cells.Drawing.ActiveXControls.ControlListStyle.Option;
            listBox.ListFillRange = "A2:A4";

            // Guardar y demostrar
            workbook.Save("ListStyleDemo.xlsx");
            Console.WriteLine("ComboBox ListStyle: " + comboBox.ListStyle);
            Console.WriteLine("ListBox ListStyle: " + listBox.ListStyle);
        }
    }
}
```

### Ver también

* enum [ControlListStyle](../../controlliststyle/)
* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


