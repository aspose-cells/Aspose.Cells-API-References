---
title: "SlicerCollection.RemoveAt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SlicerCollection. Elimina el Slicer en el índice especificado"
type: docs
url: /es/net/aspose.cells.slicers/slicercollection/removeat/
---
## SlicerCollection.RemoveAt method

Elimina el Slicer en el índice especificado

```csharp
public void RemoveAt(int index)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| índice | Int32 | El índice de posición en la colección Slicer |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class SlicerCollectionMethodRemoveAtWithInt32Demo
    {
        public static void Run()
        {
            // Crear un libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una hoja de cálculo
            Worksheet worksheet = workbook.Worksheets.Add("Sheet1");
            
            // Agrega algunos datos para la tabla pivot.
            worksheet.Cells["A1"].Value = "Fruit";
            worksheet.Cells["A2"].Value = "Apple";
            worksheet.Cells["A3"].Value = "Orange";
            worksheet.Cells["A4"].Value = "Banana";
            worksheet.Cells["B1"].Value = "Quantity";
            worksheet.Cells["B2"].Value = 10;
            worksheet.Cells["B3"].Value = 5;
            worksheet.Cells["B4"].Value = 8;

            // Agregar una tabla dinámica
            int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
            PivotTable pivotTable = worksheet.PivotTables[index];
            pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
            pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");

            // Agregar segmentadores
            Aspose.Cells.Slicers.SlicerCollection slicers = worksheet.Slicers;
            slicers.Add(pivotTable, "Fruit", "FruitSlicer1");
            slicers.Add(pivotTable, "Fruit", "FruitSlicer2");

            // Eliminar el segundo segmentador en el índice 1
            slicers.RemoveAt(1);
            
            // Guarda el libro de trabajo
            workbook.Save("SlicerCollectionMethodRemoveAtWithInt32Demo.xlsx");
        }
    }
}
```

### Ver también

* class [SlicerCollection](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)


