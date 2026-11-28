---
title: "TableToRangeOptions.LastRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "TableToRangeOptions özelliği. Tablonun son satır indeksini alır ve ayarlar"
type: docs
url: /tr/net/aspose.cells.tables/tabletorangeoptions/lastrow/
---
## TableToRangeOptions.LastRow property

Tablonun son satır indeksini alır ve ayarlar.

```csharp
public int LastRow { get; set; }
```

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Tables;

namespace AsposeCellsExamples
{
    public class TableToRangeOptionsPropertyLastRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Örnek veri oluştur
            for (int row = 0; row < 10; row++)
            {
                for (int col = 0; col < 5; col++)
                {
                    cells[row, col].PutValue($"Data {row}-{col}");
                }
            }

            // Tablo oluşturun
            int tableIndex = worksheet.ListObjects.Add(0, 0, 9, 4, true);
            ListObject table = worksheet.ListObjects[tableIndex];
            table.TableStyleType = Aspose.Cells.Tables.TableStyleType.TableStyleMedium2;

            // Tabloyu, belirtilen LastRow ile aralığa dönüştür
            TableToRangeOptions options = new TableToRangeOptions
            {
                LastRow = 7 // Only convert rows 0-7 (excluding 8-9)
            };
            table.ConvertToRange(options);

            workbook.Save("TableToRangeWithLastRow.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* class [TableToRangeOptions](../)
* namespace [Aspose.Cells.Tables](../../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../../)


