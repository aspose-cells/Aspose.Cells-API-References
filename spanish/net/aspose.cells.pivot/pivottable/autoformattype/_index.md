---
title: "PivotTable.AutoFormatType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Obtiene y establece el tipo de formato automático de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/autoformattype/
---
## PivotTable.AutoFormatType property

Obtiene y establece el tipo de formato automático de la PivotTable.

```csharp
public PivotTableAutoFormatType AutoFormatType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyAutoFormatTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Product");
            worksheet.Cells["C1"].PutValue("Sales");
            
            worksheet.Cells["A2"].PutValue("Electronics");
            worksheet.Cells["B2"].PutValue("Laptop");
            worksheet.Cells["C2"].PutValue(1200);
            
            worksheet.Cells["A3"].PutValue("Electronics");
            worksheet.Cells["B3"].PutValue("Phone");
            worksheet.Cells["C3"].PutValue(800);
            
            worksheet.Cells["A4"].PutValue("Furniture");
            worksheet.Cells["B4"].PutValue("Chair");
            worksheet.Cells["C4"].PutValue(150);
            
            // Crear tabla dinámica
            PivotTableCollection pivotTables = worksheet.PivotTables;
            int index = pivotTables.Add("A1:C4", "E5", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Agregar campos a áreas
            pivotTable.AddFieldToArea(PivotFieldType.Row, pivotTable.BaseFields["Category"]);
            pivotTable.AddFieldToArea(PivotFieldType.Column, pivotTable.BaseFields["Product"]);
            pivotTable.AddFieldToArea(PivotFieldType.Data, pivotTable.BaseFields["Sales"]);
            
            // Demostrar la propiedad AutoFormatType
            pivotTable.IsAutoFormat = true;
            pivotTable.AutoFormatType = PivotTableAutoFormatType.Report6;
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableAutoFormatTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotTableAutoFormatType](../../pivottableautoformattype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


