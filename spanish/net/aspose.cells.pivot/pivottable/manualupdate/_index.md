---
title: "PivotTable.ManualUpdate"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Indica si el informe de la tabla dinámica se recalcula solo a solicitud del usuario"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/manualupdate/
---
## PivotTable.ManualUpdate property

Indica si el informe de PivotTable se recalcula solo a petición del usuario.

```csharp
public bool ManualUpdate { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyManualUpdateDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo y completarla con datos de ejemplo
            Worksheet dataSheet = workbook.Worksheets["Sheet1"];
            dataSheet.Cells["A1"].PutValue("Category");
            dataSheet.Cells["B1"].PutValue("Value");
            dataSheet.Cells["A2"].PutValue("A");
            dataSheet.Cells["B2"].PutValue(10);
            dataSheet.Cells["A3"].PutValue("B");
            dataSheet.Cells["B3"].PutValue(20);
            dataSheet.Cells["A4"].PutValue("A");
            dataSheet.Cells["B4"].PutValue(30);

            // Agregar una tabla dinámica
            Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
            int index = pivotSheet.PivotTables.Add("Sheet1!A1:B4", "A3", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[index];

            // Configurar tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Habilitar actualización manual
            pivotTable.ManualUpdate = true;
            
            // En este punto, la tabla dinámica no se actualizará automáticamente
            Console.WriteLine("Pivot table before refresh (ManualUpdate=true):");
            Console.WriteLine(pivotSheet.Cells["B4"].StringValue); // Will be empty
            
            // Actualizar manualmente la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            Console.WriteLine("Pivot table after manual refresh:");
            Console.WriteLine(pivotSheet.Cells["B4"].StringValue); // Will show "40" (sum of category A)
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableManualUpdateDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


