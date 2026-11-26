---
title: "PivotTable.MergeLabels"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad PivotTable. Obtiene o establece si se deben combinar las etiquetas de campo de fila/columna que abarcan varias celdas"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/mergelabels/
---
## PivotTable.MergeLabels property

Obtiene o establece si se deben combinar las etiquetas de campos de fila/columna que abarcan varias celdas.

```csharp
public bool MergeLabels { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTablePropertyMergeLabelsDemo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Apple";
            worksheet.Cells["A4"].Value = "Orange";
            worksheet.Cells["A5"].Value = "Orange";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 15;
            worksheet.Cells["B4"].Value = 8;
            worksheet.Cells["B5"].Value = 12;

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            
            // Agregar campo de fila y campo de datos
            pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
            pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
            
            // Habilitar la combinación de etiquetas
            pivotTable.MergeLabels = true;
            
            // Guarda el libro de trabajo
            workbook.Save("PivotTableMergeLabelsDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


