---
title: "Enumeración PivotItemPositionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Pivot.PivotItemPositionType enum. Representa el tipo de posición del elemento base de la tabla dinámica en el campo base cuando se utiliza el cálculo ShowDataAs"
type: docs
url: /es/net/aspose.cells.pivot/pivotitempositiontype/
---
## PivotItemPositionType enumeration

Representa el tipo de posición del elemento base de la tabla dinámica en el campo base cuando se utiliza el cálculo ShowDataAs.

```csharp
public enum PivotItemPositionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Previous | `0` | Representa el elemento dinámico anterior en el PivotField. |
| Next | `1` | Representa el siguiente elemento dinámico en el PivotField. |
| Custom | `2` | Muestra los valores en un formato diferente basado en el índice del elemento dinámico en el PivotField. |

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotItemPositionTypeDemo
    {
        public static void PivotItemPositionTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");

            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar una tabla dinámica a la hoja de cálculo
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Value

            // Establece el formato de visualización de datos para mostrar los valores como diferencia respecto al elemento anterior
            PivotField dataField = pivotTable.DataFields[0];
            dataField.ShowValuesAs(PivotFieldDataDisplayFormat.DifferenceFrom, 0, PivotItemPositionType.Previous, 0);

            // Actualiza y calcula la tabla dinámica
            pivotTable.RefreshData();
            pivotTable.CalculateData();

            // Guarda el libro de trabajo
            workbook.Save("PivotItemPositionTypeExample.xlsx");

            Console.WriteLine("Pivot table created and saved successfully.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


