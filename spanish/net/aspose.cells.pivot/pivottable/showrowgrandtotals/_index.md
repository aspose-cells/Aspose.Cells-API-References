---
title: "PivotTable.ShowRowGrandTotals"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Indica si se deben mostrar totales generales para las filas de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/showrowgrandtotals/
---
## PivotTable.ShowRowGrandTotals property

Indica si se deben mostrar los totales generales para las filas de la tabla dinámica.

```csharp
public bool ShowRowGrandTotals { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyShowRowGrandTotalsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Region";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Product A";
            cells["B2"].Value = "North";
            cells["C2"].Value = 1000;
            
            cells["A3"].Value = "Product B";
            cells["B3"].Value = "South";
            cells["C3"].Value = 1500;
            
            cells["A4"].Value = "Product A";
            cells["B4"].Value = "South";
            cells["C4"].Value = 2000;
            
            cells["A5"].Value = "Product B";
            cells["B5"].Value = "North";
            cells["C5"].Value = 1200;

            // Agregar una tabla dinámica
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Configurar tabla dinámica
            pivotTable.ShowRowGrandTotals = true; // Demonstrate ShowRowGrandTotals property
            pivotTable.ShowColumnGrandTotals = true;
            
            // Agregar campos a áreas
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product as row
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Region as column
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales as data
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableShowRowGrandTotalsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


