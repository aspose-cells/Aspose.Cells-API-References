---
title: "SparklineGroupCollection.Add"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método SparklineGroupCollection. Añade un SparklineGroup con un Sparkline a la colección."
type: docs
url: /es/net/aspose.cells.charts/sparklinegroupcollection/add/
---
## Add(SparklineType) {#add}

Añade un [`SparklineGroup`](../../sparklinegroup/) con un [`Sparkline`](../../sparkline/) a la colección.

```csharp
public int Add(SparklineType type)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | SparklineType | Especifica el tipo del grupo Sparkline. |

### Valor de retorno

[`SparklineGroup`](../../sparklinegroup/) object index.

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class SparklineGroupCollectionMethodAddWithSparklineTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para sparklines
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(3);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["A4"].PutValue(2);
            worksheet.Cells["A5"].PutValue(9);

            try
            {
                // Obtén la colección de grupos sparkline
                SparklineGroupCollection sparklineGroups = worksheet.SparklineGroups;

                // Llama al método Add con el parámetro SparklineType
                int index = sparklineGroups.Add(SparklineType.Line);

                // Configura el grupo sparkline
                SparklineGroup group = sparklineGroups[index];
                group.Sparklines.Add("A1:A5", 5, 0);

                Console.WriteLine("Sparkline group added successfully with type: Line");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Guardar el resultado
            workbook.Save("SparklineGroupCollectionMethodAddWithSparklineTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [SparklineType](../../sparklinetype/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(SparklineType, string, bool, CellArea) {#add_1}

Añade un [`SparklineGroup`](../../sparklinegroup/) con algunos [`Sparkline`](../../sparkline/) a la colección.

```csharp
public int Add(SparklineType type, string dataRange, bool isVertical, CellArea locationRange)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| type | SparklineType | Especifica el tipo del grupo Sparkline. |
| dataRange | String | Especifica el rango de datos del grupo sparkline. |
| isVertical | Booleano | Especifica si se deben trazar los sparklines del rango de datos por fila o por columna. |
| locationRange | CellArea | Especifica dónde se colocarán los sparklines. |

### Valor de retorno

[`SparklineGroup`](../../sparklinegroup/) object index.

### Observaciones

Este método también creará sparklines. Si *isVertical* es verdadero, el número de filas en dataRange y locationRange debe ser el mismo. Si *isVertical* es falso, el número de columnas en dataRange y locationRange debe ser el mismo.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupCollectionMethodAddWithSparklineTypeStringBooleanCellDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra para sparklines
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(3);
            sheet.Cells["C1"].PutValue(8);
            
            // Añade un grupo sparkline con los parámetros especificados
            sheet.SparklineGroups.Add(
                SparklineType.Line, 
                "A1:C1", 
                false, 
                CellArea.CreateCellArea("D1", "D1")
            );
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* enum [SparklineType](../../sparklinetype/)
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


