---
title: "SparklineGroup.SparklineCollection"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SparklineGroup özelliği. Sparkline nesnesinin koleksiyonunu alır"
type: docs
url: /tr/net/aspose.cells.charts/sparklinegroup/sparklinecollection/
---
## SparklineGroup.SparklineCollection property

[`Sparkline`](../../sparkline/) nesnesinin koleksiyonunu alır.

```csharp
[Obsolete("Use SparklineGroup.Sparklines property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public SparklineCollection SparklineCollection { get; }
```

### Açıklamalar

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen SparklineGroup.Sparklines özelliğini kullanın. Bu özellik Kasım 2022'den itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sparklines için örnek veri ekle
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["B1"].PutValue(20);
            worksheet.Cells["C1"].PutValue(15);
            worksheet.Cells["D1"].PutValue(30);

            try
            {
                // Sparklines için konumu tanımla
                CellArea location = new CellArea
                {
                    StartRow = 0,
                    EndRow = 0,
                    StartColumn = 4,
                    EndColumn = 4
                };

                // Çalışma sayfasına bir sparkline grubu ekle
                int groupIndex = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, location);
                SparklineGroup sparklineGroup = worksheet.SparklineGroups[groupIndex];

                // Gruba bir sparkline ekle
                sparklineGroup.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

                // SparklineCollection özelliğine eriş (yalnızca okuma)
                SparklineCollection sparklineCollection = sparklineGroup.SparklineCollection;

                // Sparkline koleksiyonu hakkında bilgi göster
                Console.WriteLine($"SparklineCollection contains {sparklineCollection.Count} sparklines");

                // Koleksiyondaki sparklinelar arasında yinele
                for (int i = 0; i < sparklineCollection.Count; i++)
                {
                    Sparkline sparkline = sparklineCollection[i];
                    Console.WriteLine($"Sparkline {i + 1} location: Row {sparkline.Row}, Column {sparkline.Column}");
                }

                // Çalışma kitabını kaydedin
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

### Ayrıca Bakınız

* class [SparklineCollection](../../sparklinecollection/)
* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


