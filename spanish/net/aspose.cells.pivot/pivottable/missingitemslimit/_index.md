---
title: "PivotTable.MissingItemsLimit"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Especifica un valor booleano que indica si los campos de una tabla dinámica pueden tener varios filtros establecidos en ellos"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/missingitemslimit/
---
## PivotTable.MissingItemsLimit property

Especifica un valor booleano que indica si los campos de una PivotTable pueden tener varios filtros aplicados.

```csharp
[Obsolete("Use PivotCache.MissingItemsLimit propery  instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public PivotMissingItemLimitType MissingItemsLimit { get; set; }
```

### Observaciones

NOTA: Esta propiedad ahora está obsoleta. En su lugar, utilice la propiedad PivotCache.MissingItemsLimit. Este método será eliminado 12 meses después, a partir de septiembre de 2026. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyMissingItemsLimitDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Datos de ejemplo
            worksheet.Cells["A1"].Value = "Category";
            worksheet.Cells["B1"].Value = "Value";
            worksheet.Cells["A2"].Value = "A";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["A3"].Value = "B";
            worksheet.Cells["B3"].Value = 20;
            worksheet.Cells["A4"].Value = "C";
            worksheet.Cells["B4"].Value = 30;

            // Crear tabla dinámica y obtener la instancia
            int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:B4", "E3");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Configurar tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value
            
            // Demostrar la propiedad MissingItemsLimit
            pivotTable.MissingItemsLimit = PivotMissingItemLimitType.Max;
            
            // Actualizar datos
            pivotTable.RefreshData();
            pivotTable.CalculateData();
            
            workbook.Save("PivotTableMissingItemsLimitDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotMissingItemLimitType](../../pivotmissingitemlimittype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


