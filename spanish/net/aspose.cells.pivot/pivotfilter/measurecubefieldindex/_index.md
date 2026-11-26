---
title: "PivotFilter.MeasureCubeFieldIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotFilter. Especifica el índice del campo de cubo de medida. Esta propiedad se usa solo por filtros en pivotes OLAP y especifica en qué medida debe aplicarse un filtro de valor"
type: docs
url: /es/net/aspose.cells.pivot/pivotfilter/measurecubefieldindex/
---
## PivotFilter.MeasureCubeFieldIndex property

Especifica el índice del campo de cubo de medida. Esta propiedad se usa solo en filtros de pivotes OLAP y especifica en qué medida debe aplicarse un filtro de valor.

```csharp
public int MeasureCubeFieldIndex { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFilterPropertyMeasureCubeFieldIndexDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo y completarla con datos de ejemplo
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(1000);
            worksheet.Cells["A3"].PutValue("Banana");
            worksheet.Cells["B3"].PutValue(2000);
            worksheet.Cells["A4"].PutValue("Orange");
            worksheet.Cells["B4"].PutValue(3000);

            // Agregar una tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Agregar campos de fila y de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Actualizar los datos de la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            // Agregar un filtro a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Page, 0);
            PivotField field = pivotTable.BaseFields[0];
            
            // Crear y agregar filtro a través de PivotTable en lugar de PivotField
            int filterIndex = pivotTable.PivotFilters.Add(field.Position, PivotFilterType.Count);
            PivotFilter filter = pivotTable.PivotFilters[filterIndex];
            
            // Mostrar MeasureCubeFieldIndex
            Console.WriteLine("MeasureCubeFieldIndex: " + filter.MeasureCubeFieldIndex);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFilterMeasureCubeFieldIndexDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


