---
title: "Enumeración PivotTableSelectionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Pivot.PivotTableSelectionType. Especifica qué se puede seleccionar en una tabla dinámica durante una selección estructurada. Estas constantes pueden combinarse para seleccionar varios tipos."
type: docs
url: /es/net/aspose.cells.pivot/pivottableselectiontype/
---
## PivotTableSelectionType enumeration

Especifica qué se puede seleccionar en una tabla dinámica durante una selección estructurada. Estas constantes pueden combinarse para seleccionar varios tipos.

```csharp
public enum PivotTableSelectionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| DataAndLabel | `0` | Datos y etiquetas |
| DataOnly | `2` | Solo selecciona datos |
| LabelOnly | `1` | Solo selecciona etiquetas |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using System;

    public class PivotTableSelectionTypeDemo
    {
        public static void PivotTableSelectionTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la tabla dinámica
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["A4"].PutValue("A");
            worksheet.Cells["B4"].PutValue(200);
            worksheet.Cells["A5"].PutValue("B");
            worksheet.Cells["B5"].PutValue(250);

            // Crear una tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos a la PivotTable
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Crear un PivotArea y establecer sus propiedades
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.OnlyData = false;
            pivotArea.OnlyLabel = true;
            pivotArea.IsRowGrandIncluded = true;
            pivotArea.IsColumnGrandIncluded = true;
            pivotArea.IsOutline = false;

            // Seleccionar el área con un tipo de selección específico
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            // Guarda el libro de trabajo
            workbook.Save("PivotTableSelectionTypeExample.xlsx");

            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


