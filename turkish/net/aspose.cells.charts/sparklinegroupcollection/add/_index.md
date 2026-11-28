---
title: "SparklineGroupCollection.Add"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SparklineGroupCollection yöntemi. Bir SparklineGroup ve bir Sparkline'ı koleksiyona ekler."
type: docs
url: /tr/net/aspose.cells.charts/sparklinegroupcollection/add/
---
## Add(SparklineType) {#add}

Bir [`SparklineGroup`](../../sparklinegroup/) içinde bir [`Sparkline`](../../sparkline/) koleksiyona ekler.

```csharp
public int Add(SparklineType type)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | SparklineType | Sparkline grubunun tipini belirtir. |

### Dönüş Değeri

[`SparklineGroup`](../../sparklinegroup/) object index.

### Örnekler

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
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Sparklines için örnek veri ekle
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["A2"].PutValue(3);
            worksheet.Cells["A3"].PutValue(7);
            worksheet.Cells["A4"].PutValue(2);
            worksheet.Cells["A5"].PutValue(9);

            try
            {
                // Sparkline grup koleksiyonunu al
                SparklineGroupCollection sparklineGroups = worksheet.SparklineGroups;

                // Add yöntemini SparklineType parametresiyle çağır
                int index = sparklineGroups.Add(SparklineType.Line);

                // Sparkline grubunu yapılandır
                SparklineGroup group = sparklineGroups[index];
                group.Sparklines.Add("A1:A5", 5, 0);

                Console.WriteLine("Sparkline group added successfully with type: Line");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error executing Add method: {ex.Message}");
            }

            // Sonucu kaydet
            workbook.Save("SparklineGroupCollectionMethodAddWithSparklineTypeDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* enum [SparklineType](../../sparklinetype/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)

---

## Add(SparklineType, string, bool, CellArea) {#add_1}

Birkaç [`Sparkline`](../../sparkline/) içeren bir [`SparklineGroup`](../../sparklinegroup/) koleksiyona ekler.

```csharp
public int Add(SparklineType type, string dataRange, bool isVertical, CellArea locationRange)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | SparklineType | Sparkline grubunun tipini belirtir. |
| dataRange | String | Sparkline grubunun veri aralığını belirtir. |
| isVertical | Boolean | Sparklineları veri aralığından satır bazında mı yoksa sütun bazında mı çizeceğini belirtir. |
| locationRange | CellArea | Sparklineların nereye yerleştirileceğini belirtir. |

### Dönüş Değeri

[`SparklineGroup`](../../sparklinegroup/) object index.

### Açıklamalar

Bu yöntem aynı zamanda sparklinelar da oluşturur. *isVertical* true ise, dataRange ve locationRange içindeki satır sayısı aynı olmalıdır. *isVertical* false ise, dataRange ve locationRange içindeki sütun sayısı aynı olmalıdır.

### Örnekler

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
            
            // Sparklines için örnek veri ekle
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(3);
            sheet.Cells["C1"].PutValue(8);
            
            // Belirtilen parametrelerle sparkline grubu ekle
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

### Ayrıca Bakınız

* enum [SparklineType](../../sparklinetype/)
* struct [CellArea](../../../aspose.cells/cellarea/)
* class [SparklineGroupCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


