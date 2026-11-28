---
title: "Enum ShapePathPointValueType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Drawing.ShapePathPointValueType enum. ShapePathPoint nesnesinin değer tipini belirtir"
type: docs
url: /tr/net/aspose.cells.drawing/shapepathpointvaluetype/
---
## ShapePathPointValueType enumeration

[`ShapePathPoint`](../shapepathpoint/) nesnesinin değer tipini belirtir.

```csharp
public enum ShapePathPointValueType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Position | `0` | Nesnenin türünün konum koordinatları olduğunu belirtir. [`ShapePathPoint`](../shapepathpoint/) nesnesi bir noktanın koordinat değerlerini depolar. |
| Angle | `1` | Nesnenin türünün açı işaretçileri olduğunu belirtir. [`ShapePathPoint`](../shapepathpoint/) nesnesi yayının başlangıç ve bitiş açılarını depolar. |

### Örnekler

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
            // Demonstrasyon için yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // ShapePathPointValueType enum değerlerini göster
                ShapePathPointValueType positionType = ShapePathPointValueType.Position;
                ShapePathPointValueType angleType = ShapePathPointValueType.Angle;

                // Enum değerlerini görüntüle
                Console.WriteLine($"Position type value: {(int)positionType}");
                Console.WriteLine($"Angle type value: {(int)angleType}");

                // Enum değerlerinin beklenen sabitlerle eşleştiğini doğrulayın
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

### Ayrıca Bakınız

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


