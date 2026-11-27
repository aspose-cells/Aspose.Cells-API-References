---
title: "Enum ShapePathPointValueType"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.Drawing.ShapePathPointValueType enum. Anger värdetypen för ShapePathPoint-objektet"
type: docs
url: /sv/net/aspose.cells.drawing/shapepathpointvaluetype/
---
## ShapePathPointValueType enumeration

Anger värdetypen för [`ShapePathPoint`](../shapepathpoint/) objektet

```csharp
public enum ShapePathPointValueType
```

### Värden

| Namn | Värde | Beskrivning |
| --- | --- | --- |
| Position | `0` | Anger att objektets typ är positionskoordinater. [`ShapePathPoint`](../shapepathpoint/) objektet lagrar koordinatvärdena för en punkt. |
| Angle | `1` | Anger att objektets typ är vinkelmarkörer. [`ShapePathPoint`](../shapepathpoint/) objektet lagrar start- och slutvinklarna för bågen. |

### Exempel

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
            // Skapa en ny arbetsbok för demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Demonstrera ShapePathPointValueType enumvärden
                ShapePathPointValueType positionType = ShapePathPointValueType.Position;
                ShapePathPointValueType angleType = ShapePathPointValueType.Angle;

                // Visa enum‑värden
                Console.WriteLine($"Position type value: {(int)positionType}");
                Console.WriteLine($"Angle type value: {(int)angleType}");

                // Verifiera att enumvärdena matchar de förväntade konstanterna
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

### Se även

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


