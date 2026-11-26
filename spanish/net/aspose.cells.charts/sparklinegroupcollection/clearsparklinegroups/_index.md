---
title: "SparklineGroupCollection.ClearSparklineGroups"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SparklineGroupCollection. Elimina los grupos sparkline que se superponen a un área de celdas"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroupcollection/clearsparklinegroups/
---
## SparklineGroupCollection.ClearSparklineGroups method

Borra los grupos de sparkline que se superponen a un área de celdas.

```csharp
public void ClearSparklineGroups(CellArea cellArea)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| cellArea | CellArea | Especifica el área de celdas |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupCollectionMethodClearSparklineGroupsWithCellAreaDemo
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
                // Llama al método ClearSparklineGroups con el parámetro CellArea
                sheet.SparklineGroups.ClearSparklineGroups(ca);
                
                Console.WriteLine("Sparkline groups cleared successfully for the specified cell area.");
                
                // Verifica el recuento de grupos sparkline después de eliminar
                Console.WriteLine($"Remaining sparkline groups count: {sheet.SparklineGroups.Count}");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ClearSparklineGroups method: {ex.Message}");
            }
            
            // Guardar el resultado
            workbook.Save("ClearSparklineGroupsWithCellAreaDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


