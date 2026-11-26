---
title: "Clase PivotTableFormat"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Clase Aspose.Cells.Pivot.PivotTableFormat. Representa el formato definido en la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivottableformat/
---
## PivotTableFormat class

Representa el formato definido en la PivotTable.

```csharp
public class PivotTableFormat
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [PivotArea](../../aspose.cells.pivot/pivottableformat/pivotarea/) { get; } | Obtiene el área de la tabla dinámica. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetStyle](../../aspose.cells.pivot/pivottableformat/getstyle/)() | Obtiene el estilo formateado. |
| [SetStyle](../../aspose.cells.pivot/pivottableformat/setstyle/)(Style) | Establece el estilo del área de la tabla dinámica. |

### Ejemplos

```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;

namespace AsposeCellsExamples
{
    public class PivotTableFormatDemo
    {
        public static void RunDemo()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("Fruit");
            sheet.Cells["A3"].PutValue("Vegetable");
            sheet.Cells["B1"].PutValue("Amount");
            sheet.Cells["B2"].PutValue(50);
            sheet.Cells["B3"].PutValue(30);

            // Agregar una tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = sheet.PivotTables[pivotIndex];

            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Amount

            // Acceder a PivotTableFormatCollection
            PivotTableFormatCollection pivotFormats = pivotTable.PivotFormats;

            // Agregar un nuevo formato a la colección
            int formatIndex = pivotFormats.Add();
            PivotTableFormat pivotFormat = pivotFormats[formatIndex];

            // Acceda al PivotArea del formato
            PivotArea pivotArea = pivotFormat.PivotArea;
            pivotArea.AxisType = PivotFieldType.Data;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;

            // Crear un nuevo estilo
            Style style = workbook.CreateStyle();
            style.Font.IsBold = true;
            style.ForegroundColor = System.Drawing.Color.Yellow;
            style.Pattern = BackgroundType.Solid;

            // Aplique el estilo al PivotTableFormat
            pivotFormat.SetStyle(style);

            // Guarda el libro de trabajo
            workbook.Save("PivotTableFormatDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


