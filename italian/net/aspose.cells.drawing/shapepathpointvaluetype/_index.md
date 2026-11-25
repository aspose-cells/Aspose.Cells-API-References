---
title: "Enum ShapePathPointValueType"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Enum Aspose.Cells.Drawing.ShapePathPointValueType. Specifica il tipo di valore dell'oggetto ShapePathPoint"
type: docs
url: /it/net/aspose.cells.drawing/shapepathpointvaluetype/
---
## ShapePathPointValueType enumeration

Specifica il tipo di valore dell'oggetto [`ShapePathPoint`](../shapepathpoint/)

```csharp
public enum ShapePathPointValueType
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Position | `0` | Specifica che il tipo dell'oggetto è coordinate di posizione. L'oggetto [`ShapePathPoint`](../shapepathpoint/) memorizza i valori di coordinate di un punto. |
| Angle | `1` | Specifica che il tipo dell'oggetto è marcatori di angolo. L'oggetto [`ShapePathPoint`](../shapepathpoint/) memorizza gli angoli di inizio e fine dell'arco. |

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class DrawingClassShapePathPointValueTypeDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook per la dimostrazione
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Dimostra i valori dell'enum ShapePathPointValueType
                ShapePathPointValueType positionType = ShapePathPointValueType.Position;
                ShapePathPointValueType angleType = ShapePathPointValueType.Angle;

                // Visualizzare i valori dell'enumerazione
                Console.WriteLine($"Position type value: {(int)positionType}");
                Console.WriteLine($"Angle type value: {(int)angleType}");

                // Verifica che i valori dell'enumerazione corrispondano alle costanti previste
                Console.WriteLine($"Position equals 0: {positionType == ShapePathPointValueType.Position}");
                Console.WriteLine($"Angle equals 1: {angleType == ShapePathPointValueType.Angle}");

                Console.WriteLine("ShapePathPointValueType enum demonstrated successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with ShapePathPointValueType: {ex.Message}");
            }
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


