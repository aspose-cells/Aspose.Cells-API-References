---
title: "ComboBoxActiveXControl.ShowColumnHeads"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ComboBoxActiveXControl. Indica si se muestran los encabezados de columna"
type: docs
url: /es/net/aspose.cells.drawing.activexcontrols/comboboxactivexcontrol/showcolumnheads/
---
## ComboBoxActiveXControl.ShowColumnHeads property

Indica si se muestran los encabezados de columna.

```csharp
public bool ShowColumnHeads { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxActiveXControlPropertyShowColumnHeadsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar un control ActiveX ComboBox
            Shape shape = worksheet.Shapes.AddActiveXControl(
                Aspose.Cells.Drawing.ActiveXControls.ControlType.ComboBox, 1, 0, 1, 0, 100, 30);
            Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl comboBox = 
                (Aspose.Cells.Drawing.ActiveXControls.ComboBoxActiveXControl)shape.ActiveXControl;

            // Establecer propiedades para el ComboBox
            comboBox.ColumnCount = 2;
            comboBox.ListWidth = 100;
            
            // Agregar datos de ejemplo al ComboBox
            comboBox.ListFillRange = "A1:B3";
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue("Value1");
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue("Value2");

            // Demostrar la propiedad ShowColumnHeads
            Console.WriteLine("Initial ShowColumnHeads value: " + comboBox.ShowColumnHeads);
            
            // Habilitar encabezados de columna
            comboBox.ShowColumnHeads = true;
            Console.WriteLine("After setting ShowColumnHeads to true: " + comboBox.ShowColumnHeads);
            
            // Desactivar encabezados de columna
            comboBox.ShowColumnHeads = false;
            Console.WriteLine("After setting ShowColumnHeads to false: " + comboBox.ShowColumnHeads);

            // Guarda el libro de trabajo
            workbook.Save("ComboBoxShowColumnHeadsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ComboBoxActiveXControl](../)
* namespace [Aspose.Cells.Drawing.ActiveXControls](../../../aspose.cells.drawing.activexcontrols/)
* assembly [Aspose.Cells](../../../)


