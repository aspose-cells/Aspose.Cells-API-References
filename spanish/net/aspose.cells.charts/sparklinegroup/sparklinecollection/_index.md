---
title: "SparklineGroup.SparklineCollection"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineGroup. Obtiene la colección de objetos Sparkline"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/sparklinecollection/
---
## SparklineGroup.SparklineCollection property

Obtiene la colección del objeto [`Sparkline`](../../sparkline/).

```csharp
[Obsolete("Use SparklineGroup.Sparklines property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SparklineCollection SparklineCollection { get; }
```

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, utilice la propiedad SparklineGroup.Sparklines. Esta propiedad será eliminada 12 meses después desde noviembre de 2022. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupPropertySparklineCollectionDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para sparklines
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);
            worksheet.Cells["C1"].PutValue(15);
            worksheet.Cells["D1"].PutValue(30);

            try
            {
                // Definir la ubicación para los sparklines
                CellArea location = new CellArea
                {
                    StartRow = 0,
                    EndRow = 0,
                    StartColumn = 4,
                    EndColumn = 4
                };

                // Añade un grupo de sparkline a la hoja de cálculo
                int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, location);
                SparklineGroup sparklineGroup = worksheet.SparklineGroups[groupIndex];

                // Agregar un sparkline al grupo
                sparklineGroup.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

                // Acceder a la propiedad SparklineCollection (solo lectura)
                SparklineCollection sparklineCollection = sparklineGroup.SparklineCollection;

                // Mostrar información sobre la colección de sparklines
                Console.WriteLine($"SparklineCollection contains {sparklineCollection.Count} sparklines");

                // Iterar a través de los sparklines en la colección
                for (int i = 0; i < sparklineCollection.Count; i++)
                {
                    Sparkline sparkline = sparklineCollection[i];
                    Console.WriteLine($"Sparkline {i + 1} location: Row {sparkline.Row}, Column {sparkline.Column}");
                }

                // Guarda el libro de trabajo
                workbook.Save("SparklineCollectionDemo.xlsx");
                Console.WriteLine("SparklineCollection demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* class [SparklineCollection](../../sparklinecollection/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


