---
title: "ComboBoxActiveXControl.HideSelection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ComboBoxActiveXControl. Indica si el texto seleccionado en el control aparece resaltado cuando el control no tiene el foco"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/hideselection/
---
## ComboBoxActiveXControl.HideSelection property

Indica si el texto seleccionado en el control aparece resaltado cuando el control no tiene el foco.

```csharp
public bool HideSelection { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyHideSelectionDemo
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

            // Configurar propiedades básicas
            comboBox.ListRows = 5;
            comboBox.Value = "Select an item";
            
            // Agregar elementos de muestra usando el nombre de propiedad correcto
            comboBox.ListFillRange = "A1:A3"; // Alternative way to set items
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");

            // Demostrar la propiedad HideSelection
            comboBox.HideSelection = true; // Text won't show selection highlight when control loses focus

            // Guarda el libro de trabajo
            workbook.Save("ComboBoxHideSelectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


