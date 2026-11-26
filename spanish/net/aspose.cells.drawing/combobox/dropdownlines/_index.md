---
title: "ComboBox.DropDownLines"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ComboBox. Obtiene o establece el número de líneas de lista mostradas en la parte desplegable de un cuadro combinado"
type: docs
url: /es/net/aspose.cells.drawing/combobox/dropdownlines/
---
## ComboBox.DropDownLines property

Obtiene o establece el número de líneas de lista mostradas en la parte desplegable de un cuadro combinado.

```csharp
public int DropDownLines { get; set; }
```

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ComboBoxPropertyDropDownLinesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crear un ComboBox con los parámetros correctos
            ComboBox comboBox = worksheet.Shapes.AddComboBox(0, 0, 0, 0, 100, 100);
            comboBox.DropDownLines = 5;
            
            // Poblar las celdas de la hoja de cálculo con elementos
            worksheet.Cells["A1"].PutValue("Item 1");
            worksheet.Cells["A2"].PutValue("Item 2");
            worksheet.Cells["A3"].PutValue("Item 3");
            worksheet.Cells["A4"].PutValue("Item 4");
            worksheet.Cells["A5"].PutValue("Item 5");
            worksheet.Cells["A6"].PutValue("Item 6");

            // Vincular el cuadro combinado a los valores de las celdas
            comboBox.InputRange = "A1:A6";

            workbook.Save("ComboBoxDropDownLinesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ComboBox](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


