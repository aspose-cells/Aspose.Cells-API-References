---
title: "Enum PivotLineType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Pivot.PivotLineType. Especifica el tipo de PivotLine"
type: docs
url: /es/net/aspose.cells.pivot/pivotlinetype/
---
## PivotLineType enumeration

Especifica el tipo de PivotLine.

```csharp
public enum PivotLineType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Regular | `0` | PivotLine regular con elementos pivot. |
| Subtotal | `1` | Línea de subtotal. |
| GrandTotal | `2` | Línea de Total General. |
| Blank | `3` | Línea en blanco después de cada grupo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotLineTypeDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(300);

            // Crear tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            
            // Agregar campo de fila y campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
            
            // Ordenar campo de fila por valores en orden descendente
            pivotTable.RowFields[0].SortBy(SortOrder.Descending, 0, PivotLineType.Regular, "B2");
            
            // Calcular datos de tabla dinámica
            pivotTable.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotLineTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


