---
title: "SparklineGroup.ResetRanges"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SparklineGroup. Restablece el rango de datos y el rango de ubicación del grupo de sparklines. Este método borrará los elementos sparkline originales en el grupo y creará nuevos elementos sparkline para los nuevos rangos"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/resetranges/
---
## SparklineGroup.ResetRanges method

Restablece el rango de datos y el rango de ubicación del grupo de sparkline. Este método borrará los elementos sparkline originales en el grupo y creará nuevos elementos sparkline para los nuevos rangos.

```csharp
public void ResetRanges(string dataRange, bool isVertical, CellArea locationRange)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| dataRange | String | Especifica el nuevo rango de datos del grupo de sparklines. |
| isVertical | Booleano | Especifica si se deben trazar los sparklines del nuevo rango de datos por fila o por columna. |
| locationRange | CellArea | Especifica dónde se colocarán los sparklines. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupMethodResetRangesWithStringBooleanCellAreaDemo
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

            SparklineGroup group = sheet.SparklineGroups[idx];

            // Prepare los parámetros para ResetRanges
            string dataRange = "A1:D1";
            bool isVertical = false;
            CellArea locationRange = CellArea.CreateCellArea(6, 5, 6, 5);

            try
            {
                // Llame a ResetRanges con los parámetros (String, Boolean, CellArea)
                group.ResetRanges(dataRange, isVertical, locationRange);

                Console.WriteLine("ResetRanges method executed successfully with parameters (String, Boolean, CellArea)");
                
                
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing ResetRanges method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("SparklineGroupResetRangesDemo.xlsx");
        }
    }
}
```

### Ver también

* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


