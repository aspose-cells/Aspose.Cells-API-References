---
title: "PivotTable.ShowDetail"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método PivotTable. Muestra el detalle de un elemento en la región de datos en una nueva Tabla"
type: docs
url: /es/net/aspose.cells.pivot/pivottable/showdetail/
---
## PivotTable.ShowDetail method

Muestra el detalle de un elemento en la región de datos en una tabla nueva.

```csharp
public void ShowDetail(int rowOffset, int columnOffset, bool newSheet, int destRow, int destColumn)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| rowOffset | Int32 | Desplazamiento a la primera fila de datos en la región de datos. |
| columnOffset | Int32 | Desplazamiento a la primera columna de datos en la región de datos. |
| newSheet | Booleano | Mostrar el detalle en una nueva hoja de cálculo. |
| destRow | Int32 | La fila objetivo. |
| destColumn | Int32 | La columna objetivo. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotTableMethodShowDetailWithInt32Int32BooleanInt32Int32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo con datos de ejemplo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para la tabla dinámica
            worksheet.Cells["A1"].PutValue("Sport");
            worksheet.Cells["A2"].PutValue("Tennis");
            worksheet.Cells["A3"].PutValue("Basketball");
            worksheet.Cells["A4"].PutValue("Tennis");
            worksheet.Cells["B1"].PutValue("Score");
            worksheet.Cells["B2"].PutValue(80);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(85);

            // Crear tabla dinámica
            int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Sport");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Score");

            // Mostrar detalle para una celda específica
            pivotTable.ShowDetail(1, 0, true, 0, 0);

            // Guarda el libro de trabajo
            workbook.Save("PivotTableShowDetailExample.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


