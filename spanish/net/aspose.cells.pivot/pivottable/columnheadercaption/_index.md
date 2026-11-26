---
title: "PivotTable.ColumnHeaderCaption"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de PivotTable. Obtiene y establece el Caption personalizado del encabezado de columna de la PivotTable"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/columnheadercaption/
---
## PivotTable.ColumnHeaderCaption property

Obtiene y establece el título personalizado del encabezado de columna de la PivotTable.

```csharp
public string ColumnHeaderCaption { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyColumnHeaderCaptionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Product";
            cells["B1"].Value = "Quarter";
            cells["C1"].Value = "Sales";
            
            cells["A2"].Value = "Bike";
            cells["A3"].Value = "Bike";
            cells["A4"].Value = "Car";
            cells["A5"].Value = "Car";
            
            cells["B2"].Value = "Q1";
            cells["B3"].Value = "Q2";
            cells["B4"].Value = "Q1";
            cells["B5"].Value = "Q2";
            
            cells["C2"].Value = 1000;
            cells["C3"].Value = 2000;
            cells["C4"].Value = 3000;
            cells["C5"].Value = 4000;

            // Agregar una tabla dinámica
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Agregar campos a áreas
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Quarter
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales
            
            // Establecer el título del encabezado de columna
            PivotField columnField = pivotTable.ColumnFields[0];
            pivotTable.ColumnHeaderCaption = "Quarter Header";
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableColumnHeaderCaptionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


