---
title: "PivotTable.IsSelected"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Indica si esta PivotTable está seleccionada"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/isselected/
---
## PivotTable.IsSelected property

Indica si esta PivotTable está seleccionada.

```csharp
public bool IsSelected { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyIsSelectedDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["B2"].Value = 10;
            cells["A3"].Value = "Orange";
            cells["B3"].Value = 15;
            cells["A4"].Value = "Banana";
            cells["B4"].Value = 20;

            // Agregar una tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = sheet.PivotTables[index];

            // Inicialmente, IsSelected es falso
            Console.WriteLine("PivotTable IsSelected initially: " + pivotTable.IsSelected);

            // Seleccionar la tabla dinámica
            pivotTable.IsSelected = true;
            Console.WriteLine("PivotTable IsSelected after setting to true: " + pivotTable.IsSelected);

            // Deseleccionar la tabla dinámica
            pivotTable.IsSelected = false;
            Console.WriteLine("PivotTable IsSelected after setting to false: " + pivotTable.IsSelected);
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


