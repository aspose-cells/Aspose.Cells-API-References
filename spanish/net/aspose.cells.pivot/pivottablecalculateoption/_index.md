---
title: "Clase PivotTableCalculateOption"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Pivot.PivotTableCalculateOption. Representa las opciones de cálculo de datos de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottablecalculateoption/
---
## PivotTableCalculateOption class

Representa las opciones de cálculo de datos de la tabla dinámica.

```csharp
public class PivotTableCalculateOption
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [PivotTableCalculateOption](pivottablecalculateoption/)() | El constructor predeterminado. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [RefreshCharts](../../aspose.cells.pivot/pivottablecalculateoption/refreshcharts/) { get; set; } | Indica si los gráficos de actualización se basan en esta tabla dinámica. |
| [RefreshData](../../aspose.cells.pivot/pivottablecalculateoption/refreshdata/) { get; set; } | Indica si la fuente de datos de la tabla dinámica se actualiza. |
| [RefreshOption](../../aspose.cells.pivot/pivottablecalculateoption/refreshoption/) { get; set; } | Obtiene y establece opciones para actualizar la fuente de datos al caché de la tabla dinámica. |
| [ReserveMissingPivotItemType](../../aspose.cells.pivot/pivottablecalculateoption/reservemissingpivotitemtype/) { get; set; } | Representa cómo reservar los elementos pivot faltantes. |

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotTableCalculateOptionDemo
    {
        public static void PivotTableCalculateOptionExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agrega algunos datos para la tabla pivot.
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B3"].PutValue(30);
            sheet.Cells["A4"].PutValue("Fruit");
            sheet.Cells["B4"].PutValue(70);
            sheet.Cells["A5"].PutValue("Vegetable");
            sheet.Cells["B5"].PutValue(40);

            // Agregar una tabla dinámica a la hoja de cálculo
            int pivotIndex = sheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Configura la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Crea un objeto PivotTableCalculateOption
            PivotTableCalculateOption calculateOption = new PivotTableCalculateOption
            {
                RefreshData = true,
                RefreshCharts = true,
                ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
            };

            // Calcula los datos de la tabla dinámica con las opciones especificadas
            pivotTable.CalculateData(calculateOption);

            // Guarda el libro de trabajo
            workbook.Save("PivotTableCalculateOptionExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


