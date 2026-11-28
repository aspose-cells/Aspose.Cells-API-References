---
title: "Enum TableStyleType"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Tables.TableStyleType enum. Yerleşik tablo stil türünü temsil eder"
type: docs
url: /tr/net/aspose.cells.tables/tablestyletype/
---
## TableStyleType enumeration

Yerleşik tablo stil türünü temsil eder.

```csharp
public enum TableStyleType
```

### Değerler

| Ad | Değer | Açıklama |
| --- | --- | --- |
| None | `0` | Stil yok. |
| TableStyleLight1 | `1` | Tablo Stili Light 1 |
| TableStyleLight2 | `2` |  |
| TableStyleLight3 | `3` |  |
| TableStyleLight4 | `4` |  |
| TableStyleLight5 | `5` |  |
| TableStyleLight6 | `6` |  |
| TableStyleLight7 | `7` |  |
| TableStyleLight8 | `8` |  |
| TableStyleLight9 | `9` |  |
| TableStyleLight10 | `10` |  |
| TableStyleLight11 | `11` |  |
| TableStyleLight12 | `12` |  |
| TableStyleLight13 | `13` |  |
| TableStyleLight14 | `14` |  |
| TableStyleLight15 | `15` |  |
| TableStyleLight16 | `16` |  |
| TableStyleLight17 | `17` |  |
| TableStyleLight18 | `18` |  |
| TableStyleLight19 | `19` |  |
| TableStyleLight20 | `20` |  |
| TableStyleLight21 | `21` |  |
| TableStyleMedium1 | `22` |  |
| TableStyleMedium2 | `23` |  |
| TableStyleMedium3 | `24` |  |
| TableStyleMedium4 | `25` |  |
| TableStyleMedium5 | `26` |  |
| TableStyleMedium6 | `27` |  |
| TableStyleMedium7 | `28` |  |
| TableStyleMedium8 | `29` |  |
| TableStyleMedium9 | `30` |  |
| TableStyleMedium10 | `31` |  |
| TableStyleMedium11 | `32` |  |
| TableStyleMedium12 | `33` |  |
| TableStyleMedium13 | `34` |  |
| TableStyleMedium14 | `35` |  |
| TableStyleMedium15 | `36` |  |
| TableStyleMedium16 | `37` |  |
| TableStyleMedium17 | `38` |  |
| TableStyleMedium18 | `39` |  |
| TableStyleMedium19 | `40` |  |
| TableStyleMedium20 | `41` |  |
| TableStyleMedium21 | `42` |  |
| TableStyleMedium22 | `43` |  |
| TableStyleMedium23 | `44` |  |
| TableStyleMedium24 | `45` |  |
| TableStyleMedium25 | `46` |  |
| TableStyleMedium26 | `47` |  |
| TableStyleMedium27 | `48` |  |
| TableStyleMedium28 | `49` |  |
| TableStyleDark1 | `50` |  |
| TableStyleDark2 | `51` |  |
| TableStyleDark3 | `52` |  |
| TableStyleDark4 | `53` |  |
| TableStyleDark5 | `54` |  |
| TableStyleDark6 | `55` |  |
| TableStyleDark7 | `56` |  |
| TableStyleDark8 | `57` |  |
| TableStyleDark9 | `58` |  |
| TableStyleDark10 | `59` |  |
| TableStyleDark11 | `60` |  |
| Custom | `61` |  |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Tables;
    using System;

    public class TableStyleTypeDemo
    {
        public static void TableStyleTypeExample()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();

            // Çalışma kitabına yeni bir çalışma sayfası ekle
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma sayfasına örnek veri ekle
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["A3"].PutValue("Jane");
            worksheet.Cells["A4"].PutValue("Doe");

            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["B2"].PutValue(30);
            worksheet.Cells["B3"].PutValue(25);
            worksheet.Cells["B4"].PutValue(35);

            // Çalışma sayfasında bir ListObject (tablo) oluştur
            int listObjectIndex = worksheet.ListObjects.Add(1, 0, 4, 1, true);
            ListObject listObject = worksheet.ListObjects[listObjectIndex];

            // Tablo stil türünü ayarla
            listObject.TableStyleType = TableStyleType.TableStyleMedium2;

            // Tablo için ek özellikleri ayarlayın
            listObject.ShowHeaderRow = true;
            listObject.ShowTotals = true;
            listObject.ShowTableStyleFirstColumn = true;
            listObject.ShowTableStyleLastColumn = true;
            listObject.ShowTableStyleRowStripes = true;
            listObject.ShowTableStyleColumnStripes = true;

            // Çalışma kitabını kaydedin
            workbook.Save("TableStyleTypeExample.xlsx");

            // Tablo stil tipini çıktı olarak verin
            Console.WriteLine("Table Style Type: " + listObject.TableStyleType);
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Tables](../../aspose.cells.tables/)
* assembly [Aspose.Cells](../../)


