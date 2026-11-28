---
title: "Enum TotalsCalculation"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Tables.TotalsCalculation enum. Liste sütununun Toplamlar satırındaki hesaplama türünü belirler"
type: docs
url: /tr/net/aspose.cells.tables/totalscalculation/
---
## TotalsCalculation enumeration

Liste sütununun Toplamlar satırındaki hesaplama türünü belirler.

```csharp
public enum TotalsCalculation
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Sum | `6` | Toplamların toplam hesaplamasını temsil eder. |
| Count | `2` | Toplamların sayım hesaplamasını temsil eder. |
| Average | `1` | Toplamların ortalama hesaplamasını temsil eder. |
| Max | `4` | Toplamların maksimum hesaplamasını temsil eder. |
| Min | `5` | Min toplam hesaplamasını temsil eder. |
| Var | `8` | Var toplam hesaplamasını temsil eder. |
| CountNums | `3` | Count Nums toplam hesaplamasını temsil eder. |
| StdDev | `7` | StdDev toplam hesaplamasını temsil eder. |
| None | `0` | No toplam hesaplamasını temsil eder. |
| Custom | `9` | Özel hesaplamayı temsil eder. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TotalsCalculationDemo
    {
        public static void TotalsCalculationExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Çalışma sayfasını bazı verilerle doldurun
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 4; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Çalışma sayfasına bir tablo ekle
            ListObjectCollection tables = workbook.Worksheets[0].ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Toplam satırını göster
            table.ShowTotals = true;

            // Tablodaki beşinci sütuna eriş
            ListColumn listColumn = table.ListColumns[4];

            // TotalsCalculation özelliğini Sum olarak ayarla
            listColumn.TotalsCalculation = TotalsCalculation.Sum;

            // İsteğe bağlı olarak, sütun için bir formül ayarla
            listColumn.Formula = "=[A]";

            // Çalışma kitabını kaydedin
            workbook.Save("TotalsCalculationExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


