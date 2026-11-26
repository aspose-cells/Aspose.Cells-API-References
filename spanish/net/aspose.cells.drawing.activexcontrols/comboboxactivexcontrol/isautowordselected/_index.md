---
title: "ComboBoxActiveXControl.IsAutoWordSelected"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ComboBoxActiveXControl. Especifica la unidad básica utilizada para ampliar una selección. True indica que la unidad básica es un solo carácter. false indica que la unidad básica es una palabra completa"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/isautowordselected/
---
## ComboBoxActiveXControl.IsAutoWordSelected property

Especifica la unidad básica utilizada para ampliar una selección. True indica que la unidad básica es un solo carácter. false indica que la unidad básica es una palabra completa.

```csharp
public virtual bool IsAutoWordSelected { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Drawing.ActiveXControls;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyIsAutoWordSelectedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ComboBox con todos los parámetros requeridos
            var shape = worksheet.Shapes.AddActiveXControl(ControlType.ComboBox, 5, 0, 100, 20, 100, 20);
            ComboBoxActiveXControl comboBox = (ComboBoxActiveXControl)shape.ActiveXControl;

            // Configurar propiedades básicas
            comboBox.ListRows = 5;
            comboBox.ColumnCount = 1;
            comboBox.Value = "Sample Text";

            // Demostrar la propiedad IsAutoWordSelected
            comboBox.IsAutoWordSelected = false;
            Console.WriteLine("IsAutoWordSelected set to: " + comboBox.IsAutoWordSelected);

            // Guarda el libro de trabajo
            workbook.Save("ComboBoxIsAutoWordSelectedDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


