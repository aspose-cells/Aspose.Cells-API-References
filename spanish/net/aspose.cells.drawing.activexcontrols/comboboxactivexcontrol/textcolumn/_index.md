---
title: "ComboBoxActiveXControl.TextColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ComboBoxActiveXControl. Representa la columna en un ComboBox o ListBox que se muestra al usuario"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/textcolumn/
---
## ComboBoxActiveXControl.TextColumn property

Representa la columna en un ComboBox o ListBox que se muestra al usuario.

```csharp
public int TextColumn { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyTextColumnDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ComboBox con todos los parámetros requeridos
            var shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 
                10, 10, 150, 30, 100, 20);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Configurar las propiedades del combo box
            comboBox.ColumnCount = 2;
            comboBox.ListRows = 5;
            
            // Agregar elementos usando ListFillRange (alternativa a AddItem)
            worksheet.Cells["A1"].PutValue("Item1");
            worksheet.Cells["B1"].PutValue("Description1");
            worksheet.Cells["A2"].PutValue("Item2");
            worksheet.Cells["B2"].PutValue("Description2");
            worksheet.Cells["A3"].PutValue("Item3");
            worksheet.Cells["B3"].PutValue("Description3");
            comboBox.ListFillRange = "A1:B3";

            // Demostrar la propiedad TextColumn
            comboBox.TextColumn = 2; // Display second column (descriptions) as text
            comboBox.BoundColumn = 1; // But bind to first column (items)

            // Guarda el libro de trabajo
            workbook.Save("ComboBoxTextColumnDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


