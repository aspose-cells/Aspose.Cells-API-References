---
title: "PivotTable.PageFieldWrapCount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Obtiene el número de campos de página en cada columna o fila del informe PivotTable."
type: docs
url: /es/net/aspose.cells.pivot/pivottable/pagefieldwrapcount/
---
## PivotTable.PageFieldWrapCount property

Obtiene el número de campos de página en cada columna o fila del informe de PivotTable.

```csharp
public int PageFieldWrapCount { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyPageFieldWrapCountDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            
            // Introducir datos
            Worksheet data = workbook.Worksheets.Add("data");
            data.Cells["A1"].PutValue("Country");
            data.Cells["B1"].PutValue("Product");
            data.Cells["C1"].PutValue("Vendor");
            data.Cells["D1"].PutValue("Value");
            data.Cells["A2"].PutValue("USA");
            data.Cells["B2"].PutValue("Car");
            data.Cells["C2"].PutValue("Ford");
            data.Cells["D2"].PutValue(1200.987654321);
            data.Cells["A3"].PutValue("Japan");
            data.Cells["B3"].PutValue("Bike");
            data.Cells["C3"].PutValue("Yamaha");
            data.Cells["D3"].PutValue(985.123456789);

            // Crear tabla dinámica
            Worksheet pivot = workbook.Worksheets.Add("pivot");
            PivotTableCollection pivotTables = pivot.PivotTables;
            int index = pivotTables.Add("=data!A1:D3", "A1", "pivotTable1");
            PivotTable pivotTable = pivotTables[index];
            
            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
            pivotTable.AddFieldToArea(PivotFieldType.Column, "Product");
            pivotTable.AddFieldToArea(PivotFieldType.Page, "Vendor");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");

            // Establecer la propiedad PageFieldWrapCount
            pivotTable.PageFieldWrapCount = 2; // Number of page fields per row
            
            // Calcular y actualizar la tabla dinámica
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTablePageFieldWrapCountDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


