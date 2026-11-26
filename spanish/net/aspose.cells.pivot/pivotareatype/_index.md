---
title: "Enumeración PivotAreaType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Pivot.PivotAreaType. Indica el tipo de regla que se utiliza para describir un área o aspecto de la tabla dinámica."
type: docs
url: /es/net/aspose.cells.pivot/pivotareatype/
---
## PivotAreaType enumeration

Indica el tipo de regla que se utiliza para describir un área o aspecto de la PivotTable.

```csharp
public enum PivotAreaType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Sin área de tabla dinámica. |
| Normal | `1` | Representa un encabezado o elemento. |
| Data | `2` | Representa algo en el área de datos. |
| All | `3` | Representa toda la tabla dinámica. |
| Origin | `4` | Representa las celdas en blanco en la esquina superior izquierda de la tabla dinámica (superior derecha para hojas RTL). |
| Button | `5` | Representa un botón de campo. |
| TopRight | `6` | Representa las celdas en blanco en la esquina superior derecha de la tabla dinámica (superior izquierda para hojas RTL). |

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotAreaTypeDemo
    {
        public static void PivotAreaTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();

            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["A2"].PutValue("Apples");
            worksheet.Cells["A3"].PutValue("Oranges");
            worksheet.Cells["A4"].PutValue("Bananas");

            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(200);

            // Crear una tabla dinámica
            int pivotTableIndex = worksheet.PivotTables.Add("=A1:B4", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotTableIndex];

            // Agregar campos a la PivotTable
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Sales

            // Crear un PivotArea para la tabla dinámica
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.RuleType = PivotAreaType.Normal;
            pivotArea.OnlyData = true;
            pivotArea.IsRowGrandIncluded = true;

            // Mostrar las propiedades del PivotArea
            Console.WriteLine("Pivot Area Type: " + pivotArea.RuleType);
            Console.WriteLine("Only Data: " + pivotArea.OnlyData);
            Console.WriteLine("Is Row Grand Included: " + pivotArea.IsRowGrandIncluded);

            // Guarda el libro de trabajo
            workbook.Save("PivotAreaTypeExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


