---
title: "PivotTable.ShowPivotStyleLastColumn"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Indica si se aplica el formato de columna"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/showpivotstylelastcolumn/
---
## PivotTable.ShowPivotStyleLastColumn property

Indica si se aplica el formato de columna.

```csharp
public bool ShowPivotStyleLastColumn { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowPivotStyleLastColumnDemo
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

            // Crear tabla dinámica
            int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[index];

            // Establecer el estilo de tabla dinámica y mostrar el estilo de la última columna
            pivotTable.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium9;
            pivotTable.ShowPivotStyleLastColumn = true;

            // Guarda el libro de trabajo
            workbook.Save("PivotTableShowLastColumnStyle.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


