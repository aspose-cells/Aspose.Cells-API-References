---
title: "Clase PivotAreaFilter"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Pivot.PivotAreaFilter. Representa el filtro de PivotArea para PivotTable"
type: docs
url: /es/net/aspose.cells.pivot/pivotareafilter/
---
## PivotAreaFilter class

Representa el filtro de [`PivotArea`](../pivotarea/) para [`PivotTable`](../pivottable/).

```csharp
public class PivotAreaFilter
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PivotAreaFilter](pivotareafilter/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [FieldIndex](../../aspose.cells.pivot/pivotareafilter/fieldindex/) { get; } | Obtiene el índice del campo en los campos de origen al que se refiere este filtro. Un valor de -2 indica el campo de valores. |
| [Selected](../../aspose.cells.pivot/pivotareafilter/selected/) { get; set; } | Indica si este campo tiene selección. Solo funciona cuando la PivotTable está en vista de esquema. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [IsSubtotalSet](../../aspose.cells.pivot/pivotareafilter/issubtotalset/)(PivotFieldSubtotalType) | Obtiene qué subtotal está configurado para este filtro. |
| [SetSubtotals](../../aspose.cells.pivot/pivotareafilter/setsubtotals/)(PivotFieldSubtotalType, bool) | Subtotal para el filtro. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotClassPivotAreaFilterDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Configuración de datos de ejemplo
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Bike";
            worksheet.Cells["A3"].Value = "Car";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;
            
            // Crear PivotTable - corregir el manejo del valor de retorno
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Crear y configurar PivotAreaFilter
            PivotAreaFilter filter = new PivotAreaFilter();
            filter.Selected = true;
            filter.SetSubtotals(PivotFieldSubtotalType.Sum, true);
            
            // Demostrar métodos
            bool isSumSet = filter.IsSubtotalSet(PivotFieldSubtotalType.Sum);
            Console.WriteLine($"Sum subtotal visibility set: {isSumSet}");
            
            workbook.Save("PivotAreaFilterDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


