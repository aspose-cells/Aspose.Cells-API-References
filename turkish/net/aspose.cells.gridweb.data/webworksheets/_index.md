---
title: "WebWorksheets sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridWeb.Data.WebWorksheets sınıfı."
type: docs
url: /tr/net/aspose.cells.gridweb.data/webworksheets/
---
## WebWorksheets class

```csharp
[Obsolete("This class is obsolete; use  GridWorksheetCollection instead")]
public class WebWorksheets : ICollection, ISerializable
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [WebWorksheets](webworksheets/)(MainWeb, GridWorksheetCollection) |  |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [ActiveSheet](../../aspose.cells.gridweb.data/webworksheets/activesheet/) { get; } |  |
| [ActiveSheetIndex](../../aspose.cells.gridweb.data/webworksheets/activesheetindex/) { get; set; } |  |
| [Count](../../aspose.cells.gridweb.data/webworksheets/count/) { get; } |  |
| [DefaultFontName](../../aspose.cells.gridweb.data/webworksheets/defaultfontname/) { get; set; } |  |
| [DefaultFontSize](../../aspose.cells.gridweb.data/webworksheets/defaultfontsize/) { get; set; } |  |
| [IsFixedSize](../../aspose.cells.gridweb.data/webworksheets/isfixedsize/) { get; } | Koleksiyonun sabit bir boyuta sahip olup olmadığını gösteren bir değer alır. |
| [IsReadOnly](../../aspose.cells.gridweb.data/webworksheets/isreadonly/) { get; } | IList'in yalnızca okunur olup olmadığını gösteren bir değer alır. |
| [IsSynchronized](../../aspose.cells.gridweb.data/webworksheets/issynchronized/) { get; } | ICollection'a erişimin senkronize (iş parçacığı güvenli) olup olmadığını gösteren bir değer alır. |
| [Item](../../aspose.cells.gridweb.data/webworksheets/item/) { get; } | Belirtilen indeksteki Worksheet öğesini alır. (2 indeksleyici) |
| [PivotCaches](../../aspose.cells.gridweb.data/webworksheets/pivotcaches/) { get; } | PivotCache koleksiyon nesnesini alır |
| [PivotTables](../../aspose.cells.gridweb.data/webworksheets/pivottables/) { get; } | pivotTable koleksiyon nesnesini alır. |
| [SyncRoot](../../aspose.cells.gridweb.data/webworksheets/syncroot/) { get; } | ICollection'a erişimi senkronize etmek için kullanılabilecek bir nesne alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add)() | Koleksiyona bir çalışma sayfası ekler. |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add_1)(object) | Bir sayfa nesnesi ekler. |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add_2)(string) | Koleksiyona bir çalışma sayfası ekler. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy_1)(int) | Koleksiyona bir çalışma sayfası ekler ve mevcut bir çalışma sayfasından verileri kopyalar. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy_2)(string) | Koleksiyona bir çalışma sayfası ekler ve var olan bir çalışma sayfasından verileri kopyalar. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy)(WebWorksheet) | Koleksiyona bir çalışma sayfası ekler ve var olan bir çalışma sayfasından verileri kopyalar. |
| [Clear](../../aspose.cells.gridweb.data/webworksheets/clear/)() | Tüm çalışma sayfalarını temizler. |
| [Contains](../../aspose.cells.gridweb.data/webworksheets/contains/)(object) | Koleksiyonun sayfayı içerip içermediğini gösterir. |
| [CopyTo](../../aspose.cells.gridweb.data/webworksheets/copyto/)(Array, int) | İçeriği bir diziye kopyalar. |
| [GetEnumerator](../../aspose.cells.gridweb.data/webworksheets/getenumerator/)() |  |
| [ImportDataView](../../aspose.cells.gridweb.data/webworksheets/importdataview/#importdataview)(DataView, TableItemStyle, TableItemStyle) | Bir DataView'den içe aktarır. DataView'in tablo adını kullanarak otomatik olarak bir sayfa oluşturur. |
| [ImportDataView](../../aspose.cells.gridweb.data/webworksheets/importdataview/#importdataview_1)(DataView, TableItemStyle, TableItemStyle, string, int, int) | Bir DataView'i belirtilen sayfaya ve konuma içe aktarır. |
| [ImportExcelFile](../../aspose.cells.gridweb.data/webworksheets/importexcelfile/#importexcelfile)(Stream) | Disk dosya akışı veya bellek akışı dahil olmak üzere bir Excel dosyası akışından içe aktarır. |
| [ImportExcelFile](../../aspose.cells.gridweb.data/webworksheets/importexcelfile/#importexcelfile_1)(string) | Bir Excel dosyasından içe aktarır. |
| [IndexOf](../../aspose.cells.gridweb.data/webworksheets/indexof/)(object) | Sayfanın indeksini alır. |
| [Insert](../../aspose.cells.gridweb.data/webworksheets/insert/)(int, string) | Bir sayfayı belirtilen indekse ekler. |
| [LoadCSVFile](../../aspose.cells.gridweb.data/webworksheets/loadcsvfile/#loadcsvfile)(Stream) | CSV dosya akışından veri yükler. |
| [LoadCSVFile](../../aspose.cells.gridweb.data/webworksheets/loadcsvfile/#loadcsvfile_1)(string) | CSV dosyasından veri yükler. |
| [LoadHTMLFile](../../aspose.cells.gridweb.data/webworksheets/loadhtmlfile/#loadhtmlfile)(Stream) | HTML dosya akışından veri yükler. |
| [LoadHTMLFile](../../aspose.cells.gridweb.data/webworksheets/loadhtmlfile/#loadhtmlfile_1)(string) | HTML dosyasından veri yükler. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/loadspreadsheetmlfile/#loadspreadsheetmlfile)(Stream) | SpreadSheetML dosya akışından veri yükler. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/loadspreadsheetmlfile/#loadspreadsheetmlfile_1)(string) | SpreadSheetML dosyasından veri yükler. |
| [Remove](../../aspose.cells.gridweb.data/webworksheets/remove/)(object) | Bir sayfayı kaldırır. |
| [RemoveAt](../../aspose.cells.gridweb.data/webworksheets/removeat/#removeat)(int) | Belirtilen indeksteki sayfayı kaldırır. |
| [RemoveAt](../../aspose.cells.gridweb.data/webworksheets/removeat/#removeat_1)(string) | Belirtilen adla öğeyi kaldırır. |
| [RunAllFormulas](../../aspose.cells.gridweb.data/webworksheets/runallformulas/)() | Tüm hücrelerin formüllerini çalıştırır. |
| [SaveCSVFile](../../aspose.cells.gridweb.data/webworksheets/savecsvfile/#savecsvfile)(Stream) | Verileri CSV dosya akışına kaydeder. |
| [SaveCSVFile](../../aspose.cells.gridweb.data/webworksheets/savecsvfile/#savecsvfile_1)(string) | Verileri CSV dosyasına kaydeder. |
| [SaveHTMLFile](../../aspose.cells.gridweb.data/webworksheets/savehtmlfile/#savehtmlfile)(Stream) | Verileri HTML dosya akışına kaydeder. |
| [SaveHTMLFile](../../aspose.cells.gridweb.data/webworksheets/savehtmlfile/#savehtmlfile_1)(string) | Verileri HTML dosyasına kaydeder. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/savespreadsheetmlfile/#savespreadsheetmlfile)(Stream) | Verileri SpreadSheetML dosya akışına kaydeder. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/savespreadsheetmlfile/#savespreadsheetmlfile_1)(string) | Verileri SpreadSheetML dosyasına kaydeder. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile)(Stream) | Çalışma sayfalarını bir Excel dosya akışına kaydeder, disk IO akışı veya bellek akışı dahil. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_2)(string) | Çalışma sayfalarını Excel 2003 formatında bir Excel dosyasına kaydeder. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_1)(Stream, GridSaveFormat) | Çalışma sayfalarını bir Excel dosyasına kaydeder. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_3)(string, GridSaveFormat) | Çalışma sayfalarını bir Excel dosyasına kaydeder. |

### Açıklamalar

NOT: Bu sınıf artık kullanımdan kaldırılmıştır. Lütfen GridWorksheetCollection kullanın. Bu sınıf, Ağustos 2014'ten itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


