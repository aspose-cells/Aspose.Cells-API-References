---
title: "SparklineGroupCollection.ClearSparklines"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SparklineGroupCollection. Elimina los sparklines que están dentro de un área de celdas"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroupcollection/clearsparklines/
---
## SparklineGroupCollection.ClearSparklines method

Borra los sparklines que están dentro de un área de celdas.

```csharp
public void ClearSparklines(CellArea cellArea)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellArea | CellArea | Especifica el área de celdas |

### Observaciones

[`SparklineGroup`](../../sparklinegroup/) will be removed too if it does not contains any [`Sparkline`](../../sparkline/).

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupCollectionMethodClearSparklinesWithCellAreaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Define el CellArea para el sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Añade un grupo de sparkline a la hoja de cálculo
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);

            try
            {
                // Llama al método ClearSparklines con el parámetro CellArea
                sheet.SparklineGroups.ClearSparklines(ca);
                
                Console.WriteLine("Sparklines cleared successfully from the specified area.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearSparklines method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("SparklineGroupCollectionMethodClearSparklinesWithCellAreaDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


