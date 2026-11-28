---
title: "Sınıf TableToRangeOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Tables.TableToRangeOptions sınıfı. Tabloyu aralığa dönüştürürken seçenekleri temsil eder"
type: docs
url: /tr/net/aspose.cells.tables/tabletorangeoptions/
---
## TableToRangeOptions class

Tabloyu aralığa dönüştürürken seçenekleri temsil eder.

```csharp
public class TableToRangeOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [TableToRangeOptions](tabletorangeoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [LastRow](../../aspose.cells.tables/tabletorangeoptions/lastrow/) { get; set; } | Tablonun son satır indeksini alır ve ayarlar. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableToRangeOptionsDemo
    {
        public static void TableToRangeOptionsExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Çalışma sayfasını bazı verilerle doldurun
            for (int i = 0; i < 5; i++)
            {
                cells[0, i].PutValue(CellsHelper.ColumnIndexToName(i));
            }
            for (int row = 1; row < 10; row++)
            {
                for (int column = 0; column < 5; column++)
                {
                    cells[row, column].PutValue(row * column);
                }
            }

            // Çalışma sayfasına bir ListObject (tablo) ekle
            ListObjectCollection tables = worksheet.ListObjects;
            int index = tables.Add(0, 0, 9, 4, true);
            ListObject table = tables[index];

            // Tablonun bazı özelliklerini ayarlayın
            table.ShowTotals = true;
            table.ListColumns[4].TotalsCalculation = TotalsCalculation.Sum;

            // TableToRangeOptions bir örnek oluşturun
            TableToRangeOptions options = new TableToRangeOptions
            {
                LastRow = 9 // Set the last row index of the table
            };

            // Seçenekleri kullanarak tabloyu bir aralığa dönüştürün
            table.ConvertToRange(options);

            // Çalışma kitabını kaydedin
            workbook.Save("TableToRangeOptionsExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


