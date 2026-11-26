---
title: "CellArea.EndRow"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Campo CellArea. Obtiene o establece la fila final de esta área"
type: docs
url: /es/net/aspose.cells/cellarea/endrow/
---
## CellArea.EndRow field

Obtiene o establece la fila final de esta área.

```csharp
public int EndRow;
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class CellAreaFieldEndRowDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(150);
            
            // Agregar tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Agregar campo de fila y campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Demostrar el uso de EndRow
            Console.WriteLine("Pivot table ends at row: " + pivotTable.TableRange2.EndRow);
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTable_EndRow_Demo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


