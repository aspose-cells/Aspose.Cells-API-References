---
title: "WorksheetCollection.ClearPivottables"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método WorksheetCollection. Elimina tablas dinámicas de la hoja de cálculo"
type: docs
url: /es/net/aspose.cells/worksheetcollection/clearpivottables/
---
## WorksheetCollection.ClearPivottables method

Borra las tablas dinámicas de la hoja de cálculo.

```csharp
public void ClearPivottables()
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class WorksheetCollectionMethodClearPivottablesDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crear datos de muestra para tabla dinámica
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Agregar una tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            Aspose.Cells.Pivot.PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            Console.WriteLine("Pivot tables count before clearing: " + worksheet.PivotTables.Count);

            // Eliminar todas las tablas dinámicas de todas las hojas de cálculo
            workbook.Worksheets.ClearPivottables();

            Console.WriteLine("Pivot tables count after clearing: " + worksheet.PivotTables.Count);
        }
    }
}
```

### Ver también

* class [WorksheetCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


