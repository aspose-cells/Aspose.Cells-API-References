---
title: "DataBar.ShowValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataBar. Obtener o establecer la bandera que indica si se deben mostrar los valores de las celdas a las que se aplica esta barra de datos. El valor predeterminado es true"
type: docs
url: /es/net/aspose.cells/databar/showvalue/
---
## DataBar.ShowValue property

Obtener o establecer la bandera que indica si se deben mostrar los valores de las celdas a las que se aplica esta barra de datos. El valor predeterminado es true.

```csharp
public bool ShowValue { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DataBarPropertyShowValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].PutValue(30);
            sheet.Cells["A4"].PutValue(40);

            // Agregar formato condicional de barra de datos
            int idx = sheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = sheet.ConditionalFormattings[idx];
            CellArea area = new CellArea();
            area.StartRow = 0;
            area.EndRow = 3;
            area.StartColumn = 0;
            area.EndColumn = 0;
            fcc.AddArea(area);

            // Agregar condición de barra de datos
            int conditionIndex = fcc.AddCondition(FormatConditionType.DataBar);
            FormatCondition fc = fcc[conditionIndex];
            
            // Establecer propiedades de la barra de datos
            fc.DataBar.MinCfvo.Type = FormatConditionValueType.Min;
            fc.DataBar.MaxCfvo.Type = FormatConditionValueType.Max;
            fc.DataBar.Color = Color.Green;
            
            // Demostrar la propiedad ShowValue
            fc.DataBar.ShowValue = true; // Show cell values along with data bars
            
            // Guarda el libro de trabajo
            workbook.Save("DataBarShowValueDemo.xlsx");
            
            Console.WriteLine("DataBar ShowValue demo completed. Output file: DataBarShowValueDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DataBar](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


