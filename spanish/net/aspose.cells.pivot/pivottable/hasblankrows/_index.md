---
title: "PivotTable.HasBlankRows"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Indica si se deben agregar filas en blanco. Esta propiedad solo se aplica a los tipos de formato automático de PivotTable que requieren agregar filas en blanco"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/hasblankrows/
---
## PivotTable.HasBlankRows property

Indica si se deben agregar filas en blanco. Esta propiedad solo se aplica a los tipos de formato automático de PivotTable que requieren agregar filas en blanco.

```csharp
[Obsolete("Use PivotField.InsertBlankRow property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool HasBlankRows { get; set; }
```

### Observaciones

NOTA: Esta propiedad está ahora obsoleta. En su lugar, utilice la propiedad PivotField.InsertBlankRow. Este método será eliminado 12 meses después, a partir de abril de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyHasBlankRowsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet dataSheet = wb.Worksheets[0];
            
            // Crear datos de ejemplo
            dataSheet.Cells[0, 0].PutValue("Category");
            dataSheet.Cells[0, 1].PutValue("Product");
            dataSheet.Cells[0, 2].PutValue("Sales");
            
            Random rnd = new Random();
            for (int i = 1; i <= 10; i++)
            {
                dataSheet.Cells[i, 0].PutValue(rnd.Next(2) == 0 ? "Electronics" : "Furniture");
                dataSheet.Cells[i, 1].PutValue("Product " + rnd.Next(1, 4));
                dataSheet.Cells[i, 2].PutValue(rnd.Next(100, 1000));
            }

            // Agregar tabla dinámica
            Worksheet pivotSheet = wb.Worksheets.Add("PivotTable");
            int pivotIndex = pivotSheet.PivotTables.Add(
                "=Sheet1!A1:C11", "A1", "PivotTable1");
            PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];

            // Configurar tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Row, 1); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales
            
            // Demostrar la propiedad HasBlankRows
            pivotTable.HasBlankRows = false; // Remove blank lines between items
            
            // Guarda el libro de trabajo
            wb.Save("PivotTableHasBlankRowsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


