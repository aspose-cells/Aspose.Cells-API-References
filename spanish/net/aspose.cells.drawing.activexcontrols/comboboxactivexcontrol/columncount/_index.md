---
title: "ComboBoxActiveXControl.ColumnCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ComboBoxActiveXControl. Representa el número de columnas a mostrar en un ComboBox o ListBox"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/columncount/
---
## ComboBoxActiveXControl.ColumnCount property

Representa el número de columnas a mostrar en un ComboBox o ListBox.

```csharp
public int ColumnCount { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyColumnCountDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Fruits");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["A4"].PutValue("Cherry");

            // Agregar control ActiveX ComboBox
            var shape = worksheet.Shapes.AddActiveXControl(Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 1, 0, 1, 0, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Establecer la propiedad ColumnCount y otras propiedades
            comboBox.ColumnCount = 1;
            comboBox.ListWidth = 100;
            comboBox.Value = "Apple;Banana;Cherry";

            // Guarda el libro de trabajo
            workbook.Save("ComboBoxColumnCountDemo.xlsx");

            Console.WriteLine("ComboBox with ColumnCount=1 has been created and saved.");
        }
    }
}
```

### Ver también

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


