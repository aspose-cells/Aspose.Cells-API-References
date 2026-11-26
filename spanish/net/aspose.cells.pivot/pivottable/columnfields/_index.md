---
title: "PivotTable.ColumnFields"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Devuelve un objeto PivotFields que se muestra actualmente como campos de columna"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/columnfields/
---
## PivotTable.ColumnFields property

Devuelve un objeto PivotFields que se muestra actualmente como campos de columna.

```csharp
public PivotFieldCollection ColumnFields { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyColumnFieldsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            var cells = worksheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Sales";
            cells["A2"].Value = "Bikes";
            cells["B2"].Value = 100;
            cells["A3"].Value = "Bikes";
            cells["B3"].Value = 200;
            cells["A4"].Value = "Cars";
            cells["B4"].Value = 300;
            cells["A5"].Value = "Cars";
            cells["B5"].Value = 400;
            cells["A6"].Value = "Trucks";
            cells["B6"].Value = 500;

            // Agregar tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B6", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos de fila y columna
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Sales");

            // Acceder y manipular el campo de columna
            PivotField columnField = pivotTable.ColumnFields[0];
            columnField.FilterByValue(0, PivotFilterType.ValueGreaterThan, 300, 0);

            // Calcular y actualizar datos
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotTableColumnFieldsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFieldCollection](../../pivotfieldcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


