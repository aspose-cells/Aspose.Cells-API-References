---
title: "Sınıf AutoFilter"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.AutoFilter sınıfı. Belirtilen çalışma sayfası için otomatik filtrelemeyi temsil eder"
type: docs
url: /tr/net/aspose.cells/autofilter/
---
## AutoFilter class

Belirtilen çalışma sayfası için otomatik filtrelemeyi temsil eder.

```csharp
public class AutoFilter
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [FilterColumns](../../aspose.cells/autofilter/filtercolumns/) { get; } | Filtre sütunlarının koleksiyonunu alır. |
| [Range](../../aspose.cells/autofilter/range/) { get; set; } | Belirtilen AutoFilter'ın uygulandığı aralığı temsil eder. |
| [ShowFilterButton](../../aspose.cells/autofilter/showfilterbutton/) { get; set; } | Bu sütun için AutoFilter düğmesinin görünür olup olmadığını gösterir. |
| [Sorter](../../aspose.cells/autofilter/sorter/) { get; } | Veri sıralayıcısını alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [AddDateFilter](../../aspose.cells/autofilter/adddatefilter/)(int, DateTimeGroupingType, int, int, int, int, int, int) | Bir tarih filtresi ekler. |
| [AddFillColorFilter](../../aspose.cells/autofilter/addfillcolorfilter/)(int, BackgroundType, CellsColor, CellsColor) | Dolgu rengi filtresi ekler. |
| [AddFilter](../../aspose.cells/autofilter/addfilter/)(int, string) | Bir filtre sütunu için filtre ekler. |
| [AddFontColorFilter](../../aspose.cells/autofilter/addfontcolorfilter/)(int, CellsColor) | Yazı tipi rengi filtresi ekler. |
| [AddIconFilter](../../aspose.cells/autofilter/addiconfilter/)(int, IconSetType, int) | Bir simge filtresi ekler. |
| [Custom](../../aspose.cells/autofilter/custom/#custom)(int, FilterOperatorType, object) | Listeyi özel bir ölçüte göre filtreler. |
| [Custom](../../aspose.cells/autofilter/custom/#custom_1)(int, FilterOperatorType, object, bool, FilterOperatorType, object) | Listeyi özel ölçütlerle filtreler. |
| [DynamicFilter](../../aspose.cells/autofilter/dynamicfilter/)(int, DynamicFilterType) | Dinamik bir filtre ekler. |
| [Filter](../../aspose.cells/autofilter/filter/)(int, string) | Listeyi belirtilen ölçütlerle filtreler. |
| [FilterTop10](../../aspose.cells/autofilter/filtertop10/)(int, bool, bool, int) | Listede ilk 10 öğeyi filtrele |
| [GetCellArea](../../aspose.cells/autofilter/getcellarea/#getcellarea)() | Bu AutoFilter'ın uygulandığı [`CellArea`](../cellarea/) alır. |
| [GetCellArea](../../aspose.cells/autofilter/getcellarea/#getcellarea_1)(bool) | Belirtilen AutoFilter'ın uygulandığı [`CellArea`](../cellarea/) alır. |
| [MatchBlanks](../../aspose.cells/autofilter/matchblanks/)(int) | Listedeki tüm boş hücreleri eşleştir. |
| [MatchNonBlanks](../../aspose.cells/autofilter/matchnonblanks/)(int) | Listedeki tüm boş olmayan hücreleri eşleştir. |
| [Refresh](../../aspose.cells/autofilter/refresh/#refresh)() | Satırları gizlemek veya göstermek için otomatik filtreleri yenile. |
| [Refresh](../../aspose.cells/autofilter/refresh/#refresh_1)(bool) | Tüm gizli satırların indekslerini alır. |
| [RemoveDateFilter](../../aspose.cells/autofilter/removedatefilter/)(int, DateTimeGroupingType, int, int, int, int, int, int) | Bir tarih filtresini kaldırır. |
| [RemoveFilter](../../aspose.cells/autofilter/removefilter/#removefilter)(int) | Belirli filtreyi kaldır. |
| [RemoveFilter](../../aspose.cells/autofilter/removefilter/#removefilter_1)(int, string) | Bir filtre sütunu için filtreyi kaldırır. |
| [SetRange](../../aspose.cells/autofilter/setrange/)(int, int, int) | Belirtilen AutoFilter'ın uygulandığı aralığı ayarlar. |
| [ShowAll](../../aspose.cells/autofilter/showall/)() | Tüm satırların gizlemesini kaldır. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class AutoFilterDemo
    {
        public static void AutoFilterExample()
        {
            // Açılacak Excel dosyasını içeren bir dosya akışı oluşturma
            // Workbook nesnesi örnekleniyor
            Workbook workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Excel dosyasındaki ilk çalışma sayfasına erişim
            Worksheet worksheet = workbook.Worksheets[0];
            // Başlık satırının hücre aralığını vererek AutoFilter oluşturma
            worksheet.AutoFilter.Range = "A1:B8";
            // Belirtilen değerlerle sütunları filtreleme
            worksheet.AutoFilter.Filter(0, "Bananas");
            worksheet.AutoFilter.Refresh();

            // Değiştirilmiş Excel dosyasını kaydetme.
            workbook.Save("AutoFilterExample.xlsx");
            workbook.Save("AutoFilterExample.pdf");

            // Workbook nesnesi örnekleniyor
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Excel dosyasındaki ilk çalışma sayfasına erişim
            worksheet = workbook.Worksheets[0];

            // AutoFilter'ın diğer işlevlerini göstermek için ek kod
            // AutoFilter için aralığı ayarlama
            worksheet.AutoFilter.Range = "A1:B8";
            // Bir filtre ekleme
            worksheet.AutoFilter.AddFilter(0, "Apples");
            // Tarih filtresi ekleme
            worksheet.AutoFilter.AddDateFilter(1, DateTimeGroupingType.Year, 2022, 0, 0, 0, 0, 0);

            worksheet.AutoFilter.Refresh();
            // Değiştirilmiş Excel dosyasını kaydetme.
            workbook.Save("AutoFilterExample2.xlsx");
            workbook.Save("AutoFilterExample2.pdf");

            // Workbook nesnesi örnekleniyor
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Excel dosyasındaki ilk çalışma sayfasına erişim
            worksheet = workbook.Worksheets[0];
                        
            // Yazı tipi rengi filtresi ekleme
            CellsColor color = workbook.CreateCellsColor();
            color.Color = System.Drawing.Color.Red;

            worksheet.AutoFilter.AddFontColorFilter(0, color);

            worksheet.AutoFilter.Refresh();
            // Değiştirilmiş Excel dosyasını kaydetme.
            workbook.Save("AutoFilterExample3.xlsx");
            workbook.Save("AutoFilterExample3.pdf");

            // Workbook nesnesi örnekleniyor
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Excel dosyasındaki ilk çalışma sayfasına erişim
            worksheet = workbook.Worksheets[0];

            // Dolgu rengi filtresi ekleme
            CellsColor foregroundColor = workbook.CreateCellsColor();
            foregroundColor.Color = System.Drawing.Color.Red;
            CellsColor backgroundColor = workbook.CreateCellsColor();
            backgroundColor.Color = System.Drawing.Color.White;

            worksheet.AutoFilter.AddFillColorFilter(0, BackgroundType.Solid, foregroundColor, backgroundColor);

            worksheet.AutoFilter.Refresh();
            // Değiştirilmiş Excel dosyasını kaydetme.
            workbook.Save("AutoFilterExample4.xlsx");
            workbook.Save("AutoFilterExample4.pdf");

            // Workbook nesnesi örnekleniyor
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Excel dosyasındaki ilk çalışma sayfasına erişim
            worksheet = workbook.Worksheets[0];

            // Boşları eşleştirme
            worksheet.AutoFilter.MatchBlanks(0);

            worksheet.AutoFilter.Refresh();
            // Değiştirilmiş Excel dosyasını kaydetme.
            workbook.Save("AutoFilterExample5.xlsx");
            workbook.Save("AutoFilterExample5.pdf");

            // Workbook nesnesi örnekleniyor
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Excel dosyasındaki ilk çalışma sayfasına erişim
            worksheet = workbook.Worksheets[0];

            // Boş olmayanları eşleştirme
            worksheet.AutoFilter.MatchNonBlanks(0);

            worksheet.AutoFilter.Refresh();
            // Değiştirilmiş Excel dosyasını kaydetme.
            workbook.Save("AutoFilterExample6.xlsx");
            workbook.Save("AutoFilterExample6.pdf");

            // Workbook nesnesi örnekleniyor
            workbook = new Workbook("AutoFilterExampleTemplate.xlsx");
            // Excel dosyasındaki ilk çalışma sayfasına erişim
            worksheet = workbook.Worksheets[0];

            // Özel filtre
            worksheet.AutoFilter.Custom(0, FilterOperatorType.Contains, "Test");

            worksheet.AutoFilter.Refresh();
            // Değiştirilmiş Excel dosyasını kaydetme.
            workbook.Save("AutoFilterExample7.xlsx");
            workbook.Save("AutoFilterExample7.pdf");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


