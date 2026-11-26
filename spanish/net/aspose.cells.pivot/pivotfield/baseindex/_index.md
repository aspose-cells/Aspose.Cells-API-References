---
title: "PivotField.BaseIndex"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotField. Representa el índice en los campos dinámicos de origen."
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/baseindex/
---
## PivotField.BaseIndex property

Representa el índice en los campos de tabla dinámica de origen.

```csharp
public int BaseIndex { get; set; }
```

### Observaciones

NOTA: Este asignador de esta propiedad está ahora obsoleto. Este asignador de esta propiedad será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyBaseIndexDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[wb.Worksheets.Add()];
            ws.Name = "PivotData";
            
            // Datos de ejemplo
            ws.Cells["A1"].PutValue("Category");
            ws.Cells["B1"].PutValue("Quarter");
            ws.Cells["C1"].PutValue("Sales");
            
            ws.Cells["A2"].PutValue("Electronics");
            ws.Cells["A3"].PutValue("Electronics");
            ws.Cells["A4"].PutValue("Clothing");
            ws.Cells["A5"].PutValue("Clothing");
            
            ws.Cells["B2"].PutValue("Q1");
            ws.Cells["B3"].PutValue("Q2");
            ws.Cells["B4"].PutValue("Q1");
            ws.Cells["B5"].PutValue("Q2");
            
            ws.Cells["C2"].PutValue(1000);
            ws.Cells["C3"].PutValue(1200);
            ws.Cells["C4"].PutValue(800);
            ws.Cells["C5"].PutValue(900);

            // Crear tabla dinámica - corregido obteniendo la PivotTable desde el índice.
            int pivotIndex = ws.PivotTables.Add("=PivotData!A1:C5", "E3", "PivotTable1");
            PivotTable pt = ws.PivotTables[pivotIndex];
            
            // Agregar campo de fila
            int rowIndex = pt.AddFieldToArea(PivotFieldType.Row, "Category");
            PivotField rowField = pt.RowFields[rowIndex];
            
            // Agregar campo de columna (se usará como campo base)
            int colIndex = pt.AddFieldToArea(PivotFieldType.Column, "Quarter");
            PivotField quarterField = pt.ColumnFields[colIndex];
            
            // Agregar campo de datos con cálculo normal
            int dataIndex = pt.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField dataField = pt.DataFields[dataIndex];
            dataField.Function = ConsolidationFunction.Sum;
            
            // Agregar segundo campo de datos que muestra la diferencia con el trimestre anterior
            int diffIndex = pt.AddFieldToArea(PivotFieldType.Data, "Sales");
            PivotField diffField = pt.DataFields[diffIndex];
            diffField.DisplayName = "QoQ Difference";
            diffField.ShowValuesAs(
                PivotFieldDataDisplayFormat.DifferenceFrom, 
                quarterField.BaseIndex, 
                PivotItemPositionType.Previous,
                0);
            
            // Calcular y guardar
            wb.CalculateFormula();
            wb.Save("PivotTableWithBaseIndexDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


