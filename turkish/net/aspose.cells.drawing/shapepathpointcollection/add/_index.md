---
title: "ShapePathPointCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ShapePathPointCollection yöntemi. EMU biriminde bir yol noktasını ekler"
type: docs
url: /tr/net/aspose.cells.drawing/shapepathpointcollection/add/
---
## ShapePathPointCollection.Add method

EMU biriminde bir yol noktasını ekler.

```csharp
[Obsolete("Use the MoveTo,LineTo,CubicBezierTo and ArcTo methods in ShapePath instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add(int x, int y)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| x | Int32 | x koordinatı. |
| y | Int32 | y koordinatı. |

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine, ShapePath içindeki MoveTo,LineTo,CubicBezierTo ve ArcTo yöntemlerini kullanın. Bu yöntem, Ağustos 2025'ten itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class ShapePathPointCollectionMethodAddWithInt32Int32Demo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Bir şekil yolu nokta koleksiyonu oluşturun
            ShapePathPointCollection pathPoints = new ShapePathPointCollection();

            try
            {
                // Add yöntemini (Int32, Int32) parametreleriyle çağırın
                pathPoints.Add(50, 10);
                pathPoints.Add(50, 50);
                pathPoints.Add(10, 50);

                // Bir şekil yolu oluştur ve noktaları ekle
                ShapePath path = new ShapePath();

                // Başlangıç noktasına git
                path.MoveTo(10, 10);

                foreach (ShapePathPoint point in pathPoints)
                {
                    path.LineTo(point.X, point.Y);
                }
                path.Close();

                // Yapılandırılmış yol ile serbest şekil ekleyin
                Shape shape = worksheet.Shapes.AddFreeform(
                    topRow: 2,
                    top: 0,
                    leftColumn: 2,
                    left: 0,
                    height: 200,
                    width: 200,
                    paths: new ShapePath[] { path }
                );

                // Sonucu kaydet
                workbook.Save("ShapePathPointCollectionMethodAddWithInt32Int32Demo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }
        }
    }
}
```

### Ayrıca Bakınız

* class [ShapePathPointCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


