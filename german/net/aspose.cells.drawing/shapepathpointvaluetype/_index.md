---
title: "Aufzählung ShapePathPointValueType"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Drawing.ShapePathPointValueType enum. Gibt den Werttyp des ShapePathPoint-Objekts an"
type: docs
url: /de/net/aspose.cells.drawing/shapepathpointvaluetype/
---
## ShapePathPointValueType enumeration

Gibt den Werttyp des [`ShapePathPoint`](../shapepathpoint/)-Objekts an

```csharp
public enum ShapePathPointValueType
```

### Werte

| Name | Wert | Beschreibung |
| --- | --- | --- |
| Position | `0` | Gibt an, dass der Typ des Objekts Positionskoordinaten ist. Das [`ShapePathPoint`](../shapepathpoint/)-Objekt speichert die Koordinatenwerte eines Punktes. |
| Angle | `1` | Gibt an, dass der Typ des Objekts Winkelmarkierungen ist. Das [`ShapePathPoint`](../shapepathpoint/)-Objekt speichert die Start- und Endwinkel des Bogens. |

### Beispiele

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
            // Erstellt ein neues Arbeitsbuch für die Demonstration
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Demonstrieren Sie die Werte des ShapePathPointValueType-Enums
                ShapePathPointValueType positionType = ShapePathPointValueType.Position;
                ShapePathPointValueType angleType = ShapePathPointValueType.Angle;

                // Die Enum-Werte anzeigen
                Console.WriteLine($"Position type value: {(int)positionType}");
                Console.WriteLine($"Angle type value: {(int)angleType}");

                // Überprüfen Sie, ob die Enum-Werte den erwarteten Konstanten entsprechen
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

### Siehe auch

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


