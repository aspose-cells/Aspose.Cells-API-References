---
title: "Enum TableDataSourceType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Tables.TableDataSourceType enum. Tabloların veri kaynağı türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.tables/tabledatasourcetype/
---
## TableDataSourceType enumeration

Tablonun veri kaynağı türünü temsil eder.

```csharp
public enum TableDataSourceType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| Worksheet | `0` | Excel Çalışma Sayfası Tablosu |
| SharePoint | `1` | Okuma-yazma SharePoint bağlantılı Listesi |
| XML | `2` | XML eşleyici Tablosu |
| QueryTable | `3` | Sorgu Tablosu |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableDataSourceTypeDemo
    {
        public static void TableDataSourceTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("ID");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);

            worksheet.Cells["B1"].PutValue("Name");
            worksheet.Cells["B2"].PutValue("Alice");
            worksheet.Cells["B3"].PutValue("Bob");
            worksheet.Cells["B4"].PutValue("Charlie");

            // Çalışma sayfasına bir ListObject (tablo) ekle
            int listObjectIndex = worksheet.ListObjects.Add(1, 0, 4, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];

            // Tablonun görüntüleme adını ayarla
            listObject.DisplayName = "SampleTable";

            // Tablonun veri kaynağı türünü ayarla
            TableDataSourceType dataSourceType = listObject.DataSourceType;

            // Veri kaynağı türünü çıktı ver
            Console.WriteLine("Data Source Type: " + dataSourceType);

            // Çalışma kitabını kaydedin
            workbook.Save("TableDataSourceTypeExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


