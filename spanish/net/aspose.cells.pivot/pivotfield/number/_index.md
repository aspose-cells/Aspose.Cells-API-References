---
title: "PivotField.Number"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "PivotField property. Representa el formato de visualización incorporado de números y fechas"
type: docs
url: /es/net/aspose.cells.pivot/pivotfield/number/
---
## PivotField.Number property

Representa el formato de visualización incorporado de números y fechas.

```csharp
public int Number { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotFieldPropertyNumberDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            sheet.Cells["A1"].PutValue("Date");
            sheet.Cells["A2"].PutValue(new DateTime(2023, 1, 8));
            sheet.Cells["A3"].PutValue(new DateTime(2023, 1, 15));
            sheet.Cells["A4"].PutValue(new DateTime(2023, 1, 22));
            
            // Crear tabla dinámica
            int pivotIndex = sheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
            PivotTable pivot = sheet.PivotTables[pivotIndex];
            
            // Agregar campo de fecha al área de columnas y establecer formato numérico
            int fieldIndex = pivot.AddFieldToArea(PivotFieldType.Column, 0);
            PivotField field = pivot.ColumnFields[fieldIndex];
            field.Number = 16; // d-mmm format
            
            // Actualizar y calcular la tabla dinámica
            pivot.RefreshData();
            pivot.CalculateData();
            
            // Guarda el libro de trabajo
            workbook.Save("PivotFieldNumberDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


