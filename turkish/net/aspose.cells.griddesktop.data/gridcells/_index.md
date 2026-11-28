---
title: "Sınıf GridCells"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridDesktop.Data.GridCells sınıfı. Hücre nesnelerinin bir koleksiyonunu kapsar"
type: docs
url: /tr/net/aspose.cells.griddesktop.data/gridcells/
---
## GridCells class

Cell nesnelerinin bir koleksiyonunu kapsar.

```csharp
public class GridCells : IEnumerable
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Columns](../../aspose.cells.griddesktop.data/gridcells/columns/) { get; } |  |
| [Count](../../aspose.cells.griddesktop.data/gridcells/count/) { get; } | Hücre sayısını alır. |
| [FirstCell](../../aspose.cells.griddesktop.data/gridcells/firstcell/) { get; } | Bu çalışma sayfasındaki ilk hücreyi alır. |
| [Item](../../aspose.cells.griddesktop.data/gridcells/item/) { get; } | Belirtilen hücre satır indeksi ve sütun indeksindeki [`GridCell`](../gridcell/) öğesini alır. (2 indeksleyici) |
| [LastCell](../../aspose.cells.griddesktop.data/gridcells/lastcell/) { get; } | Bu çalışma sayfasındaki son hücreyi alır. |
| [MaxColumn](../../aspose.cells.griddesktop.data/gridcells/maxcolumn/) { get; } | Veri veya stil içeren hücrenin maksimum sütun indeksi. |
| [MaxDataColumn](../../aspose.cells.griddesktop.data/gridcells/maxdatacolumn/) { get; } | Veri içeren hücrenin maksimum sütun indeksi. |
| [MaxDataRow](../../aspose.cells.griddesktop.data/gridcells/maxdatarow/) { get; } | Veri içeren hücrenin maksimum satır indeksi. |
| [MaxRow](../../aspose.cells.griddesktop.data/gridcells/maxrow/) { get; } | Veri veya stil içeren hücrenin maksimum satır indeksi. |
| [MergedCells](../../aspose.cells.griddesktop.data/gridcells/mergedcells/) { get; } | Birleştirilmiş hücrelerin koleksiyonunu alır. |
| [MinColumn](../../aspose.cells.griddesktop.data/gridcells/mincolumn/) { get; } | Koleksiyonda oluşturulmuş hücrelerin minimum sütun indeksi (tüm sütun için stil tanımlı ancak içinde hücre oluşturulmamış sütunu içermez). |
| [MinDataColumn](../../aspose.cells.griddesktop.data/gridcells/mindatacolumn/) { get; } | Veri içeren hücrenin minimum sütun indeksi. |
| [MinDataRow](../../aspose.cells.griddesktop.data/gridcells/mindatarow/) { get; } | Veri içeren hücrenin minimum satır indeksi. |
| [MinRow](../../aspose.cells.griddesktop.data/gridcells/minrow/) { get; } | Veri veya stil içeren hücrenin minimum satır indeksi. |
| [RowEnumerator](../../aspose.cells.griddesktop.data/gridcells/rowenumerator/) { get; } | Satırların enumerator'ünü alır |
| [Rows](../../aspose.cells.griddesktop.data/gridcells/rows/) { get; } | Bu çalışma sayfasındaki bireysel satırları temsil eden [`GridRow`](../gridrow/) nesnelerinin koleksiyonunu alır. |
| [StandardHeight](../../aspose.cells.griddesktop.data/gridcells/standardheight/) { get; set; } | Bu çalışma sayfasındaki varsayılan satır yüksekliğini alır veya ayarlar, birim olarak puan. |
| [StandardHeightPixels](../../aspose.cells.griddesktop.data/gridcells/standardheightpixels/) { get; set; } | Bu çalışma sayfasındaki varsayılan satır yüksekliğini alır veya ayarlar, birim olarak piksel. |
| [StandardWidth](../../aspose.cells.griddesktop.data/gridcells/standardwidth/) { get; set; } | Çalışma sayfasındaki varsayılan sütun genişliğini alır veya ayarlar, birim olarak karakter. |
| [StandardWidthInch](../../aspose.cells.griddesktop.data/gridcells/standardwidthinch/) { get; set; } |  |
| [StandardWidthPixels](../../aspose.cells.griddesktop.data/gridcells/standardwidthpixels/) { get; set; } |  |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [CheckCell](../../aspose.cells.griddesktop.data/gridcells/checkcell/)(int, int) | Belirtilen hücre satır indeksi ve sütun indeksindeki [`GridCell`](../gridcell/) öğesini veya null değerini alır. |
| [CheckRow](../../aspose.cells.griddesktop.data/gridcells/checkrow/)(int) | Belirtilen hücre satır indeksindeki [`GridRow`](../gridrow/) öğesini veya null değerini alır. |
| [Clear](../../aspose.cells.griddesktop.data/gridcells/clear/)() | Koleksiyondaki tüm hücreleri temizle. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents/#clearcontents)(GridCellArea) | Bir aralığın içeriğini temizler. |
| [ClearContents](../../aspose.cells.griddesktop.data/gridcells/clearcontents/#clearcontents_1)(int, int, int, int) | Bir aralığın içeriğini temizler. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats/#clearformats)(GridCellArea) | Bir aralığın biçimlendirmesini temizler. |
| [ClearFormats](../../aspose.cells.griddesktop.data/gridcells/clearformats/#clearformats_1)(int, int, int, int) | Bir aralığın biçimlendirmesini temizler. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange/#clearrange)(GridCellArea) | Bir aralığın içeriğini ve biçimlendirmesini temizler. |
| [ClearRange](../../aspose.cells.griddesktop.data/gridcells/clearrange/#clearrange_1)(int, int, int, int) | Bir aralığın içeriğini ve biçimlendirmesini temizler. |
| [CopyColumn](../../aspose.cells.griddesktop.data/gridcells/copycolumn/)(GridCells, int, int) | Bir bütün sütunun veri ve biçimlendirmesini kopyalar. |
| [CopyColumns](../../aspose.cells.griddesktop.data/gridcells/copycolumns/)(GridCells, int, int, int) | Bir bütün sütunun veri ve biçimlendirmesini kopyalar. |
| [CopyRow](../../aspose.cells.griddesktop.data/gridcells/copyrow/)(GridCells, int, int) | Bir bütün satırın veri ve biçimlendirmesini kopyalar. |
| [CopyRows](../../aspose.cells.griddesktop.data/gridcells/copyrows/)(GridCells, int, int, int) | Bazı bütün satırların veri ve biçimlendirmesini kopyalar. |
| [DeleteBlankColumns](../../aspose.cells.griddesktop.data/gridcells/deleteblankcolumns/)() | Veri içermeyen tüm boş sütunları sil. |
| [DeleteBlankRows](../../aspose.cells.griddesktop.data/gridcells/deleteblankrows/)() | Veri içermeyen tüm boş satırları sil. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn/#deletecolumn)(int) | Bir sütunu siler. |
| [DeleteColumn](../../aspose.cells.griddesktop.data/gridcells/deletecolumn/#deletecolumn_1)(int, bool) | Bir sütunu siler. |
| [DeleteColumns](../../aspose.cells.griddesktop.data/gridcells/deletecolumns/)(int, int, bool) | Birçok sütunu siler. |
| [DeleteRow](../../aspose.cells.griddesktop.data/gridcells/deleterow/)(int) | Bir satırı siler. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows/#deleterows)(int, int) | Birkaç satırı siler. |
| [DeleteRows](../../aspose.cells.griddesktop.data/gridcells/deleterows/#deleterows_1)(int, int, bool) | Çalışma sayfasındaki birden fazla satırı siler. |
| [GetCellStyle](../../aspose.cells.griddesktop.data/gridcells/getcellstyle/)(int, int) | Verilen hücrenin stilini al. |
| [GetColumn](../../aspose.cells.griddesktop.data/gridcells/getcolumn/)(int) | Belirtilen hücre sütun indeksindeki [`GridColumn`](../gridcolumn/) öğesini alır. |
| [GetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidth/)(int) | Belirtilen sütunun genişliğini alır |
| [GetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthinch/)(int) | Belirtilen sütunun genişliğini, birim olarak inç cinsinden alır. |
| [GetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getcolumnwidthpixel/)(int) | Belirtilen sütunun genişliğini, birim olarak piksel cinsinden alır. |
| [GetEnumerator](../../aspose.cells.griddesktop.data/gridcells/getenumerator/)() | Satırların enumerator'ünü alır |
| [GetRow](../../aspose.cells.griddesktop.data/gridcells/getrow/)(int) | Belirtilen hücre satır indeksindeki [`GridRow`](../gridrow/) öğesini alır. |
| [GetRowHeight](../../aspose.cells.griddesktop.data/gridcells/getrowheight/)(int) | Belirtilen bir satırın yüksekliğini alır. |
| [GetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/getrowheightinch/)(int) | Belirtilen bir satırın yüksekliğini inç biriminde alır. |
| [GetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/getrowheightpixel/)(int) | Belirtilen bir satırın yüksekliğini piksel biriminde alır. |
| [GetViewColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/getviewcolumnwidthpixel/)(int) | Farklı görünüm tipinde genişliği al. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns/#groupcolumns)(int, int) | Sütunları gruplar. |
| [GroupColumns](../../aspose.cells.griddesktop.data/gridcells/groupcolumns/#groupcolumns_1)(int, int, bool) | Sütunları gruplar. |
| [GroupRows](../../aspose.cells.griddesktop.data/gridcells/grouprows/)(int, int) | Satırları gruplar. |
| [HideColumn](../../aspose.cells.griddesktop.data/gridcells/hidecolumn/)(int) | Bir sütunu gizler. |
| [HideColumns](../../aspose.cells.griddesktop.data/gridcells/hidecolumns/)(int, int) | Birden fazla sütunu gizler. |
| [HideRow](../../aspose.cells.griddesktop.data/gridcells/hiderow/)(int) | Bir satırı gizler. |
| [HideRows](../../aspose.cells.griddesktop.data/gridcells/hiderows/)(int, int) | Birden fazla satırı gizler. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn/#insertcolumn)(int) | Çalışma sayfasına yeni bir sütun ekler. |
| [InsertColumn](../../aspose.cells.griddesktop.data/gridcells/insertcolumn/#insertcolumn_1)(int, bool) | Çalışma sayfasına yeni bir sütun ekler. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns/#insertcolumns)(int, int) | Çalışma sayfasına bazı sütunlar ekler. |
| [InsertColumns](../../aspose.cells.griddesktop.data/gridcells/insertcolumns/#insertcolumns_1)(int, int, bool) | Çalışma sayfasına bazı sütunlar ekler. |
| [InsertRow](../../aspose.cells.griddesktop.data/gridcells/insertrow/)(int) | Çalışma sayfasına yeni bir satır ekler. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows/#insertrows)(int, int) | Çalışma sayfasına birden fazla satır ekler. |
| [InsertRows](../../aspose.cells.griddesktop.data/gridcells/insertrows/#insertrows_1)(int, int, bool) | Çalışma sayfasına birden fazla satır ekler. |
| [IsBlankColumn](../../aspose.cells.griddesktop.data/gridcells/isblankcolumn/)(int) | Verilen sütunun boş olup olmadığını kontrol eder (herhangi bir veri içermez). |
| [IsColumnHidden](../../aspose.cells.griddesktop.data/gridcells/iscolumnhidden/)(int) | Verilen indeksteki sütunun gizli olup olmadığını kontrol eder. |
| [IsRowHidden](../../aspose.cells.griddesktop.data/gridcells/isrowhidden/)(int) | Verilen indeksteki satırın gizli olup olmadığını kontrol eder. |
| [Merge](../../aspose.cells.griddesktop.data/gridcells/merge/)(int, int, int, int) | Belirtilen hücre aralığını tek bir hücrede birleştirir. |
| [RemoveFormulas](../../aspose.cells.griddesktop.data/gridcells/removeformulas/)() | Tüm formülleri kaldırır ve formülün değeriyle değiştirir. |
| [SetColumnWidth](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidth/)(int, double) | Belirtilen sütunun genişliğini ayarlar. |
| [SetColumnWidthInch](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthinch/)(int, double) | Sütun genişliğini inç biriminde ayarlar. |
| [SetColumnWidthPixel](../../aspose.cells.griddesktop.data/gridcells/setcolumnwidthpixel/)(int, int) | Sütun genişliğini piksel biriminde ayarlar. |
| [SetRowHeight](../../aspose.cells.griddesktop.data/gridcells/setrowheight/)(int, double) | Belirtilen satırın yüksekliğini ayarlar. |
| [SetRowHeightInch](../../aspose.cells.griddesktop.data/gridcells/setrowheightinch/)(int, double) | Satır yüksekliğini inç biriminde ayarlar. |
| [SetRowHeightPixel](../../aspose.cells.griddesktop.data/gridcells/setrowheightpixel/)(int, int) | Satır yüksekliğini piksel biriminde ayarlar. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle)(CellRange, Style) | Stili belirtilen hücre aralığına uygular. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle_2)(string, Style) | Stili belirtilen hücre aralığına uygular. |
| [SetStyle](../../aspose.cells.griddesktop.data/gridcells/setstyle/#setstyle_1)(int, int, int, int, Style) | Stili belirtilen hücre aralığına uygular. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort/#sort)(int, int, int, int, int, bool, bool, bool) | Belirtilen sütun indeksine göre bir Çalışma Sayfası aralığındaki verileri yukarıdan aşağıya artan/azalan şekilde sıralar. Belirtilen satır indeksine göre bir Çalışma Sayfası aralığındaki verileri soldan sağa artan/azalan şekilde sıralar. |
| [Sort](../../aspose.cells.griddesktop.data/gridcells/sort/#sort_1)(int, int, int, int, int[], SortOrder[], SortOrientation, bool) | Alan verilerini sıralar. |
| [SortAsNumber](../../aspose.cells.griddesktop.data/gridcells/sortasnumber/)(int, int, int, int, int[], SortOrder[], SortOrientation) | Alan verilerini (anahtar sütun verileri sayı olmalıdır) sıralar. |
| [UngroupColumns](../../aspose.cells.griddesktop.data/gridcells/ungroupcolumns/)(int, int) | Sütunların gruplamasını kaldırır. |
| [UngroupRows](../../aspose.cells.griddesktop.data/gridcells/ungrouprows/)(int, int) | Satırların gruplamasını kaldırır. |
| [UnhideColumn](../../aspose.cells.griddesktop.data/gridcells/unhidecolumn/)(int, double) | Bir sütunu gösterir. |
| [UnhideColumns](../../aspose.cells.griddesktop.data/gridcells/unhidecolumns/)(int, int, double) | Birden çok sütunu gösterir. |
| [UnhideRow](../../aspose.cells.griddesktop.data/gridcells/unhiderow/)(int, int) | Bir satırı gösterir. |
| [UnhideRows](../../aspose.cells.griddesktop.data/gridcells/unhiderows/)(int, int, double) | Gizli satırları gösterir. |
| [UnMerge](../../aspose.cells.griddesktop.data/gridcells/unmerge/)(int, int, int, int) | Belirtilen birleştirilmiş hücre aralığının birleştirmesini kaldırır. |
| static [CellIndexToName](../../aspose.cells.griddesktop.data/gridcells/cellindextoname/)(int, int) | Satır ve sütun indekslerine göre hücre adını alır. |
| static [CellNameToIndex](../../aspose.cells.griddesktop.data/gridcells/cellnametoindex/)(string, out int, out int) | Hücrenin adını temel alarak satır ve sütun indekslerini alır. |
| static [ColumnIndexToName](../../aspose.cells.griddesktop.data/gridcells/columnindextoname/)(int) | Sütun indeksine göre sütun adını alır. |
| static [ColumnNameToIndex](../../aspose.cells.griddesktop.data/gridcells/columnnametoindex/)(string) | Sütun adına göre sütun indeksini alır. |

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridDesktop.Data](../../aspose.cells.griddesktop.data/)
* assembly [Aspose.Cells.GridDesktop](../../)


