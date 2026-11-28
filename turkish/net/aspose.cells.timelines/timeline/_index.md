---
title: "Timeline sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Timelines.Timeline sınıfı. Timeline Görünümünün özet açıklaması. MS Excel 2003 Timeline'ı desteklemediği için"
type: docs
url: /tr/net/aspose.cells.timelines/timeline/
---
## Timeline class

Zaman Çizelgesi Görünümü için özet açıklama: MS Excel nedeniyle, Excel 2003 zaman çizelgesini desteklemez.

```csharp
public class Timeline
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Caption](../../aspose.cells.timelines/timeline/caption/) { get; set; } | Bu Timeline'ın başlığını alır veya ayarlar. |
| [CurrentLevel](../../aspose.cells.timelines/timeline/currentlevel/) { get; set; } | Timeline'ın mevcut zaman seviyesi. |
| [HeightPixel](../../aspose.cells.timelines/timeline/heightpixel/) { get; set; } | (**Obsolete.**) Belirtilen timeline'ın yüksekliğini piksel cinsinden alır veya ayarlar. |
| [LeftPixel](../../aspose.cells.timelines/timeline/leftpixel/) { get; set; } | (**Obsolete.**) Timeline şeklinin sol sütundan yatay ofsetini piksel cinsinden alır veya ayarlar. |
| [Name](../../aspose.cells.timelines/timeline/name/) { get; set; } | Belirtilen Timeline'ın adını alır veya ayarlar |
| [SelectionLevel](../../aspose.cells.timelines/timeline/selectionlevel/) { get; set; } | Timeline için mevcut seçimin yapıldığı zaman seviyesini alır ve ayarlar. |
| [Shape](../../aspose.cells.timelines/timeline/shape/) { get; } | Bu Timeline ile ilişkili [`TimelineShape`](../../aspose.cells.drawing/timelineshape/) nesnesini döndürür. |
| [ShowHeader](../../aspose.cells.timelines/timeline/showheader/) { get; set; } | Bu timeline'ın başlığının gösterilip gösterilmeyeceğini belirtir. |
| [ShowHorizontalScrollbar](../../aspose.cells.timelines/timeline/showhorizontalscrollbar/) { get; set; } | Yatay kaydırma çubuğunun gösterilip gösterilmeyeceğini belirtir. |
| [ShowSelectionLabel](../../aspose.cells.timelines/timeline/showselectionlabel/) { get; set; } | Seçim etiketinin gösterilip gösterilmeyeceğini belirtir. |
| [ShowTimeLevel](../../aspose.cells.timelines/timeline/showtimelevel/) { get; set; } | Zaman seviyesinin açılır seçim kutusunun gösterilip gösterilmeyeceğini belirtir. |
| [StartDate](../../aspose.cells.timelines/timeline/startdate/) { get; set; } | Bu `Timeline` öğesinin zaman aralığı kaydırma konumunun başlangıç tarihini alır ve ayarlar. |
| [TopPixel](../../aspose.cells.timelines/timeline/toppixel/) { get; set; } | (**Obsolete.**) Zaman çizelgesi şeklinin üst satırından dikey ofsetini piksel cinsinden alır veya ayarlar. |
| [WidthPixel](../../aspose.cells.timelines/timeline/widthpixel/) { get; set; } | (**Obsolete.**) Belirtilen zaman çizelgesinin genişliğini piksel cinsinden alır veya ayarlar. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [GetSelectedDateTimeRange](../../aspose.cells.timelines/timeline/getselecteddatetimerange/)() | Seçili tarih saat aralığını alır. |
| [Select](../../aspose.cells.timelines/timeline/select/)(DateTime, DateTime, bool) | Tarih saat arasındaki öğeyi seç. |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Pivot;
    using Aspose.Cells.Timelines;
    using System;

    public class TimelineDemo
    {
        public static void TimelineExample()
        {
            // Yeni bir çalışma kitabı oluşturun ve ilk çalışma sayfasını alın.
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Çalışma sayfasını örnek verilerle doldur.
            cells[0, 0].Value = "fruit";
            cells[1, 0].Value = "grape";
            cells[2, 0].Value = "blueberry";
            cells[3, 0].Value = "kiwi";
            cells[4, 0].Value = "cherry";

            // Tarih stilini oluştur.
            Style dateStyle = new CellsFactory().CreateStyle();
            dateStyle.Custom = "m/d/yyyy";
            cells[0, 1].Value = "date";
            cells[1, 1].Value = new DateTime(2021, 2, 5);
            cells[2, 1].Value = new DateTime(2022, 3, 8);
            cells[3, 1].Value = new DateTime(2023, 4, 10);
            cells[4, 1].Value = new DateTime(2024, 5, 16);
            // Tarih stilini ayarla.
            cells[1, 1].SetStyle(dateStyle);
            cells[2, 1].SetStyle(dateStyle);
            cells[3, 1].SetStyle(dateStyle);
            cells[4, 1].SetStyle(dateStyle);

            cells[0, 2].Value = "amount";
            cells[1, 2].Value = 50;
            cells[2, 2].Value = 60;
            cells[3, 2].Value = 70;
            cells[4, 2].Value = 80;

            // Bir PivotTable ekle.
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C5", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "date");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // PivotTable verilerini yenile.
            pivot.RefreshData();
            pivot.CalculateData();

            // PivotTable'ı veri kaynağı olarak kullanarak yeni bir Timeline ekle.
            sheet.Timelines.Add(pivot, 10, 5, "date");

            // Timeline nesnesini al.
            Timeline timelineObj = sheet.Timelines[0];

            // Timeline'ın özelliklerini ayarla.
            timelineObj.Caption = "timeline caption test";
            timelineObj.Name = "timeline name test";
            timelineObj.LeftPixel = 100;
            timelineObj.TopPixel = 50;
            timelineObj.WidthPixel = 300;
            timelineObj.HeightPixel = 100;

            // Çalışma kitabını kaydedin
            book.Save("TimelineExample.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Timelines](../../aspose.cells.timelines/)
* assembly [Aspose.Cells](../../)


