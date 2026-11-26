---
title: "PivotTable.CalculateRange"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método de PivotTable. Calcula el rango de las tablas dinámicas"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/calculaterange/
---
## PivotTable.CalculateRange method

Calcula el rango de la tabla dinámica.

```csharp
public void CalculateRange()
```

### Observaciones

Si este método no ha sido llamado, tal vez el rango de la tabla dinámica no esté corregido.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodCalculateRangeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar datos de muestra a la primera hoja de cálculo
            Worksheet dataSheet = workbook.Worksheets[0];
            dataSheet.Cells["A1"].PutValue("Product");
            dataSheet.Cells["B1"].PutValue("Sales");
            dataSheet.Cells["A2"].PutValue("Apple");
            dataSheet.Cells["B2"].PutValue(1000);
            dataSheet.Cells["A3"].PutValue("Banana");
            dataSheet.Cells["B3"].PutValue(2000);
            dataSheet.Cells["A4"].PutValue("Orange");
            dataSheet.Cells["B4"].PutValue(3000);

            // Agregar una tabla dinámica
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
            int pivotIndex = pivotSheet.PivotTables.Add("A1", "A1:B4", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
            
            // Agregar campos de fila y de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Calcular rango y actualizar datos
            pivotTable.CalculateRange();
            pivotTable.CalculateData();
            pivotTable.RefreshData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableCalculateRangeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


