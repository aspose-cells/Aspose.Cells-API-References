---
title: "Clase PivotTableRefreshOption"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Pivot.PivotTableRefreshOption. Representa las opciones de actualización de la fuente de datos de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottablerefreshoption/
---
## PivotTableRefreshOption class

Representa las opciones de actualización de la fuente de datos de la tabla dinámica.

```csharp
public class PivotTableRefreshOption
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PivotTableRefreshOption](pivottablerefreshoption/)() | Representa las opciones de actualización de la fuente de datos de la tabla dinámica. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [IsKeepOriginalOrder](../../aspose.cells.pivot/pivottablerefreshoption/iskeeporiginalorder/) { get; set; } | Indica si se debe mantener el orden original de los elementos pivot como en la fuente de datos anterior. |
| [KeepCachedLocalGroupData](../../aspose.cells.pivot/pivottablerefreshoption/keepcachedlocalgroupdata/) { get; set; } | Indica si se deben conservar los datos de grupo local en caché si los valores máximo y mínimo permanecen sin cambios. El valor predeterminado es false, lo que significa actualizar el grupo con la configuración local. |
| [ReserveMissingPivotItemType](../../aspose.cells.pivot/pivottablerefreshoption/reservemissingpivotitemtype/) { get; set; } | Representa cómo reservar los elementos pivot faltantes. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableRefreshOptionDemo
    {
        public static void PivotTableRefreshOptionExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells[0, 0].Value = "Fruit";
            worksheet.Cells[0, 1].Value = "Year";
            worksheet.Cells[0, 2].Value = "Amount";
            worksheet.Cells[1, 0].Value = "Apple";
            worksheet.Cells[1, 1].Value = 2020;
            worksheet.Cells[1, 2].Value = 50;
            worksheet.Cells[2, 0].Value = "Banana";
            worksheet.Cells[2, 1].Value = 2020;
            worksheet.Cells[2, 2].Value = 60;
            worksheet.Cells[3, 0].Value = "Apple";
            worksheet.Cells[3, 1].Value = 2021;
            worksheet.Cells[3, 2].Value = 70;
            worksheet.Cells[4, 0].Value = "Banana";
            worksheet.Cells[4, 1].Value = 2021;
            worksheet.Cells[4, 2].Value = 80;

            // Agregar una tabla dinámica a la hoja de cálculo
            int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
            pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
            pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount

            // Cree una instancia de PivotTableRefreshOption
            PivotTableRefreshOption refreshOption = new PivotTableRefreshOption
            {
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Actualice la tabla dinámica con las opciones especificadas
            pivotTable.RefreshData(refreshOption);
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotTableRefreshOptionExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


