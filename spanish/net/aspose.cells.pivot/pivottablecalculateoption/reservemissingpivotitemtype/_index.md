---
title: "PivotTableCalculateOption.ReserveMissingPivotItemType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTableCalculateOption. Representa cómo reservar elementos de tabla dinámica faltantes"
type: docs
url: /es/net/aspose.cells.pivot/pivottablecalculateoption/reservemissingpivotitemtype/
---
## PivotTableCalculateOption.ReserveMissingPivotItemType property

Representa cómo reservar los elementos pivot faltantes.

```csharp
public ReserveMissingPivotItemType ReserveMissingPivotItemType { get; set; }
```

### Observaciones

Solo funciona cuando [`RefreshData`](../refreshdata/) es verdadero.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionPropertyReserveMissingPivotItemTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Datos de ejemplo
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["A4"].PutValue("A");
            sheet.Cells["B4"].PutValue(30);

            // Crear tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Configurar campos de tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Establecer opciones de cálculo con ReserveMissingPivotItemType
            PivotTableCalculateOption options = new PivotTableCalculateOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Calcular con opciones
            pivotTable.CalculateData(options);

            // Guardar resultado
            workbook.Save("PivotTableReserveMissingItemsDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ReserveMissingPivotItemType](../../reservemissingpivotitemtype/)
* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


