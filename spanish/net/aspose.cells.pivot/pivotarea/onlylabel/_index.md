---
title: "PivotArea.OnlyLabel"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotArea. Indica si solo se seleccionan las etiquetas de datos para una selección de elemento"
type: docs
url: /es/net/aspose.cells.pivot/pivotarea/onlylabel/
---
## PivotArea.OnlyLabel property

Indica si solo se seleccionan las etiquetas de datos para una selección de elemento.

```csharp
public bool OnlyLabel { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaPropertyOnlyLabelDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B3", "D1", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];

            // Agregar campos
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Configurar el área de pivote
            PivotArea pivotArea = new PivotArea(pivotTable);
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.OnlyLabel = true; // Key property demonstration
            
            // Aplicar selección
            pivotArea.Select(PivotFieldType.Row, 0, PivotTableSelectionType.LabelOnly);

            workbook.Save("PivotAreaOnlyLabelDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


