---
title: "SparklineCollection.Remove"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SparklineCollection. Elimina el sparkline"
type: docs
url: /es/net/aspose.cells.charts/sparklinecollection/remove/
---
## SparklineCollection.Remove method

Elimina la sparkline

```csharp
[Obsolete("Use SparklineCollection.RemoveSparkline(Sparkline) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void Remove(object o)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| o | Objeto |  |

### Observaciones

NOTA: Este miembro está ahora obsoleto. En su lugar, por favor use el método RemoveSparkline(). Este método será eliminado 6 meses después de diciembre de 2025. Aspose se disculpa por cualquier inconveniente que haya experimentado.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineCollectionMethodRemoveWithObjectDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo y obtener la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Insertar datos de muestra en la hoja de cálculo
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);


            // Define el CellArea donde se agregarán las sparklines
            CellArea cellArea = new CellArea { StartColumn = 4, EndColumn = 4, StartRow = 0, EndRow = 0 };

            // Agregar un nuevo SparklineGroup a la hoja de cálculo
            int sparklineGroupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, cellArea);
            SparklineGroup sparklineGroup = worksheet.SparklineGroups[sparklineGroupIndex];

            SparklineCollection sparklineCollection = sparklineGroup.Sparklines;

            // Agregar sparklines al SparklineGroup
            sparklineCollection.Add("A1:D1", 0, 5);

            Console.WriteLine("Sparkline count: " + sparklineCollection.Count);

            // Establecer varias propiedades para el SparklineGroup
            sparklineGroup.ShowHighPoint = true;
            sparklineGroup.ShowLowPoint = true;

            // Establecer colores para los puntos altos y bajos
            CellsColor highPointColor = workbook.CreateCellsColor();
            highPointColor.Color = System.Drawing.Color.Green;
            sparklineGroup.HighPointColor = highPointColor;

            CellsColor lowPointColor = workbook.CreateCellsColor();
            lowPointColor.Color = System.Drawing.Color.Red;
            sparklineGroup.LowPointColor = lowPointColor;

            // Establecer el color de la serie y el grosor de la línea
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = System.Drawing.Color.Orange;
            sparklineGroup.SeriesColor = seriesColor;
            sparklineGroup.LineWeight = 1.0;


            // Obtener el primer sparkline para eliminar
            Sparkline sparklineToRemove = sparklineCollection[0];

            // Llame al método Remove con el objeto sparkline
            sparklineCollection.Remove(sparklineToRemove);

            Console.WriteLine("Sparkline removed successfully");


            Console.WriteLine("after deleted---Sparkline count: " + sparklineCollection.Count);
            // Guarda el libro de trabajo
            workbook.Save("SparklineRemoveDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SparklineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


