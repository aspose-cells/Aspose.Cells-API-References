---
title: "Slicer.AddPivotConnection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método Slicer. Añade una conexión a PivotTable"
type: docs
url: /es/net/aspose.cells.slicers/slicer/addpivotconnection/
---
## Slicer.AddPivotConnection method

Agrega una conexión de tabla dinámica.

```csharp
public void AddPivotConnection(PivotTable pivot)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| pivote | PivotTable | El objeto PivotTable |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;

namespace AsposeCellsExamples
{
    public class SlicerMethodAddPivotConnectionWithPivotTableDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra para la tabla dinámica
            Cells cells = sheet.Cells;
            cells["A1"].Value = "Fruit";
            cells["B1"].Value = "Quantity";
            cells["A2"].Value = "Apple";
            cells["A3"].Value = "Orange";
            cells["A4"].Value = "Banana";
            cells["B2"].Value = 10;
            cells["B3"].Value = 15;
            cells["B4"].Value = 5;

            // Crear tabla dinámica
            PivotTableCollection pivotTables = sheet.PivotTables;
            int index = pivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = pivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Agregar slicer - parámetros corregidos
            int slicerIndex = sheet.Slicers.Add(pivotTable, 0, 0, "Slicer1");
            Slicer slicer = sheet.Slicers[slicerIndex];

            // Agregar conexión de pivote al slicer
            slicer.AddPivotConnection(pivotTable);

            // Guarda el libro de trabajo
            workbook.Save("SlicerAddPivotConnectionDemo.xlsx");
        }
    }
}
```

### Ver también

* class [PivotTable](../../../aspose.cells.pivot/pivottable/)
* class [Slicer](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


