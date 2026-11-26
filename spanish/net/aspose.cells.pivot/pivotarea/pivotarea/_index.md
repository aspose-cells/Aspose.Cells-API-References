---
title: "PivotArea.PivotArea"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Constructor de PivotArea. Presenta el área seleccionada de la tabla dinámica"
type: docs
url: /es/net/aspose.cells.pivot/pivotarea/pivotarea/
---
## PivotArea constructor

Presenta el área seleccionada de la PivotTable.

```csharp
public PivotArea(PivotTable table)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| tabla | PivotTable |  |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotAreaMethodctorWithPivotTableDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].Value = "Product";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Sales";
            worksheet.Cells["B2"].Value = 1000;
            worksheet.Cells["B3"].Value = 2000;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E5", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregar campos a la tabla dinámica
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);

            // Demostrar el constructor de PivotArea con el parámetro PivotTable
            PivotArea pivotArea = new PivotArea(pivotTable);
            
            // Configurar el área de pivote
            pivotArea.AxisType = PivotFieldType.Row;
            pivotArea.RuleType = PivotAreaType.Normal;
            
            // Guarda el libro de trabajo
            workbook.Save("PivotAreaDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../../pivottable/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


