---
title: Slicer
second_title: Aspose.Cells for .NET API Referansı
description: Dilimleyici Görünümünün özet açıklaması
type: docs
weight: 5630
url: /tr/net/aspose.cells.slicers/slicer/
---
## Slicer class

Dilimleyici Görünümü'nün özet açıklaması

```csharp
public class Slicer
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AlternativeText](../../aspose.cells.slicers/slicer/alternativetext) { get; set; } | Slicer nesnesinin açıklayıcı (alternatif) metin dizesini döndürür veya ayarlar. |
| [Caption](../../aspose.cells.slicers/slicer/caption) { get; set; } | Belirtilen dilimleyicinin başlığını döndürür veya ayarlar. |
| [CaptionVisible](../../aspose.cells.slicers/slicer/captionvisible) { get; set; } | Dilimleyici Caption'ı görüntüleyen başlığın görünür olup olmadığını döndürür veya ayarlar varsayılan değer true |
| [ColumnWidth](../../aspose.cells.slicers/slicer/columnwidth) { get; set; } | Dilimleyicideki her sütunun genişliğini nokta olarak döndürür veya ayarlar. |
| [ColumnWidthPixel](../../aspose.cells.slicers/slicer/columnwidthpixel) { get; set; } | Dilimleyicinin her sütunu için piksel birimi cinsinden genişliği alır veya ayarlar. |
| [Height](../../aspose.cells.slicers/slicer/height) { get; set; } | Belirtilen dilimleyicinin yüksekliğini nokta olarak döndürür veya ayarlar. |
| [HeightPixel](../../aspose.cells.slicers/slicer/heightpixel) { get; set; } | Belirtilen dilimleyicinin yüksekliğini piksel cinsinden döndürür veya ayarlar. |
| [IsLocked](../../aspose.cells.slicers/slicer/islocked) { get; set; } | Dilimleyici şeklinin kilitli olup olmadığını gösterir. |
| [IsPrintable](../../aspose.cells.slicers/slicer/isprintable) { get; set; } | Dilimleyici nesnesinin yazdırılabilir olup olmadığını gösterir. |
| [LeftPixel](../../aspose.cells.slicers/slicer/leftpixel) { get; set; } | Dilimleyici şeklinin sol sütunundan piksel cinsinden yatay uzaklığını döndürür veya ayarlar. |
| [LockedAspectRatio](../../aspose.cells.slicers/slicer/lockedaspectratio) { get; set; } | En boy oranının kilitlenip kilitlenmediğini gösterir. |
| [LockedPosition](../../aspose.cells.slicers/slicer/lockedposition) { get; set; } | Belirtilen dilimleyicinin kullanıcı arabirimi kullanılarak taşınıp taşınamayacağını veya yeniden boyutlandırılabileceğini gösterir. |
| [Name](../../aspose.cells.slicers/slicer/name) { get; set; } | Belirtilen dilimleyicinin adını döndürür veya ayarlar |
| [NumberOfColumns](../../aspose.cells.slicers/slicer/numberofcolumns) { get; set; } | Belirtilen dilimleyicideki sütun sayısını döndürür veya ayarlar. |
| [Parent](../../aspose.cells.slicers/slicer/parent) { get; } | Dilimleyiciyi içeren sayfayı temsil eden Çalışma Sayfası nesnesini döndürür. Salt okunur. |
| [Placement](../../aspose.cells.slicers/slicer/placement) { get; set; } | Çizim nesnesinin altındaki hücrelere eklenme şeklini temsil eder. Özellik, bir nesnenin çalışma sayfasındaki yerleşimini kontrol eder. |
| [RowHeight](../../aspose.cells.slicers/slicer/rowheight) { get; set; } | Belirtilen dilimleyicideki her satırın yüksekliğini nokta olarak döndürür veya ayarlar. |
| [RowHeightPixel](../../aspose.cells.slicers/slicer/rowheightpixel) { get; set; } | Belirtilen dilimleyicideki her satırın yüksekliğini piksel cinsinden döndürür veya ayarlar. |
| [SlicerCache](../../aspose.cells.slicers/slicer/slicercache) { get; } | Dilimleyiciyle ilişkili SlicerCache nesnesini döndürür. Salt okunur. |
| [StyleType](../../aspose.cells.slicers/slicer/styletype) { get; set; } | Yerleşik dilimleyici style türünü belirtin, varsayılan tür SlicerStyleLight1 |
| [Title](../../aspose.cells.slicers/slicer/title) { get; set; } | Geçerli Slicer nesnesinin başlığını belirtir. |
| [TopPixel](../../aspose.cells.slicers/slicer/toppixel) { get; set; } | Dilimleyici şeklinin üst satırından piksel cinsinden dikey kaymasını döndürür veya ayarlar. |
| [Width](../../aspose.cells.slicers/slicer/width) { get; set; } | Belirtilen dilimleyicinin genişliğini nokta olarak döndürür veya ayarlar. |
| [WidthPixel](../../aspose.cells.slicers/slicer/widthpixel) { get; set; } | Belirtilen dilimleyicinin genişliğini piksel cinsinden döndürür veya ayarlar. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [AddPivotConnection](../../aspose.cells.slicers/slicer/addpivotconnection)(PivotTable) | PivotTable bağlantısı ekler. |
| [Refresh](../../aspose.cells.slicers/slicer/refresh)() | Dilimleyiciyi yenileme. Bu arada, Göreli PivotTable'ları Yenileme ve Hesaplama. |
| [RemovePivotConnection](../../aspose.cells.slicers/slicer/removepivotconnection)(PivotTable) | PivotTable bağlantısını kaldırır. |

### Örnekler

```csharp

[C#]

Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
cells[0, 0].Value = "fruit";
cells[1, 0].Value = "grape";
cells[2, 0].Value = "blueberry";
cells[3, 0].Value = "kiwi";
cells[4, 0].Value = "cherry";
cells[5, 0].Value = "grape";
cells[6, 0].Value = "blueberry";
cells[7, 0].Value = "kiwi";
cells[8, 0].Value = "cherry";

cells[0, 1].Value = "year";
cells[1, 1].Value = 2020;
cells[2, 1].Value = 2020;
cells[3, 1].Value = 2020;
cells[4, 1].Value = 2020;
cells[5, 1].Value = 2021;
cells[6, 1].Value = 2021;
cells[7, 1].Value = 2021;
cells[8, 1].Value = 2021;

cells[0, 2].Value = "amount";
cells[1, 2].Value = 50;
cells[2, 2].Value = 60;
cells[3, 2].Value = 70;
cells[4, 2].Value = 80;
cells[5, 2].Value = 90;
cells[6, 2].Value = 100;
cells[7, 2].Value = 110;
cells[8, 2].Value = 120;

PivotTableCollection pivots = sheet.PivotTables;

int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
pivot.AddFieldToArea(PivotFieldType.Column, "year");
pivot.AddFieldToArea(PivotFieldType.Data, "amount");

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;
pivot.RefreshData();
pivot.CalculateData();

SlicerCollection slicers = sheet.Slicers;
int slicerIndex = slicers.Add(pivot, "E12", "fruit");
Slicer slicer = slicers[slicerIndex];
slicer.StyleType = SlicerStyleType.SlicerStyleLight2;

SlicerCacheItemCollection items = slicer.SlicerCache.SlicerCacheItems;
SlicerCacheItem item = items[0];
item.Selected = false;
//işini yap
book.Save("out.xlsx");

[Visual Basic]

Dim book As Workbook = New Workbook()
Dim sheet As Worksheet = book.Worksheets(0)
Dim cells As Cells = sheet.Cells

cells(0, 0).Value = "fruit"
cells(1, 0).Value = "grape"
cells(2, 0).Value = "blueberry"
cells(3, 0).Value = "kiwi"
cells(4, 0).Value = "cherry"
cells(5, 0).Value = "grape"
cells(6, 0).Value = "blueberry"
cells(7, 0).Value = "kiwi"
cells(8, 0).Value = "cherry"

cells(0, 1).Value = "year"
cells(1, 1).Value = 2020
cells(2, 1).Value = 2020
cells(3, 1).Value = 2020
cells(4, 1).Value = 2020
cells(5, 1).Value = 2021
cells(6, 1).Value = 2021
cells(7, 1).Value = 2021
cells(8, 1).Value = 2021

cells(0, 2).Value = "amount"
cells(1, 2).Value = 50
cells(2, 2).Value = 60
cells(3, 2).Value = 70
cells(4, 2).Value = 80
cells(5, 2).Value = 90
cells(6, 2).Value = 100
cells(7, 2).Value = 110
cells(8, 2).Value = 120

Dim pivots As PivotTableCollection = sheet.PivotTables
Dim pivotIndex As Int32 = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable")
Dim pivot As PivotTable = pivots(pivotIndex)
pivot.AddFieldToArea(PivotFieldType.Row, "fruit")
Pivot.AddFieldToArea(PivotFieldType.Column, "year")
Pivot.AddFieldToArea(PivotFieldType.Data, "amount")

pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10
pivot.RefreshData()
pivot.CalculateData()

Dim slicers As SlicerCollection = sheet.Slicers
Dim slicerIndex As Int32 = slicers.Add(pivot, "E12", "fruit")
Dim slicer As Slicer = slicers(slicerIndex)
slicer.StyleType = SlicerStyleType.SlicerStyleLight2

Dim items As SlicerCacheItemCollection = slicer.SlicerCache.SlicerCacheItems
Dim item As SlicerCacheItem = items(0)
item.Selected = False

book.Save("out_vb.xlsx")
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells.Slicers](../../aspose.cells.slicers)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
