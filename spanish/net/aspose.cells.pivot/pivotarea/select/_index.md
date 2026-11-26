---
title: "PivotArea.Select"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotArea. Selecciona el área con filtros"
type: docs
url: /es/net/aspose.cells.pivot/pivotarea/select/
---
## PivotArea.Select method

Selecciona el área con filtros.

```csharp
public void Select(PivotFieldType axisType, int fieldPosition, 
    PivotTableSelectionType selectionType)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| axisType | PivotFieldType | La región de la PivotTable a la que se aplica esta regla. |
| fieldPosition | Int32 | Posición del campo dentro del eje al que se aplica esta regla. |
| selectionType | PivotTableSelectionType | Especifica qué se puede seleccionar en una PivotTable durante una selección estructurada. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaMethodSelectWithPivotFieldTypeInt32PivotTableSDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            workbook.Save("PivotAreaSelectDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [PivotFieldType](../../pivotfieldtype/)
* enum [PivotTableSelectionType](../../pivottableselectiontype/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


