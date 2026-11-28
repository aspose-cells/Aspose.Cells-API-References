---
title: "WebCells sınıfı"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridWeb.Data.WebCells sınıfı."
type: docs
url: /tr/net/aspose.cells.gridweb.data/webcells/
---
## WebCells class

```csharp
[Obsolete("This class is obsolete; use  GridCells instead")]
public class WebCells
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/webcells/count/) { get; } | Hücre sayısını alır. |
| [Item](../../aspose.cells.gridweb.data/webcells/item/) { get; } | Belirtilen hücre satır indeksi ve sütun indeksindeki Cell öğesini alır. (2 indeksleyici) |
| [MaxColumn](../../aspose.cells.gridweb.data/webcells/maxcolumn/) { get; } |  |
| [MaxRow](../../aspose.cells.gridweb.data/webcells/maxrow/) { get; } |  |
| [MergedCells](../../aspose.cells.gridweb.data/webcells/mergedcells/) { get; } | Birleştirilmiş hücrelerin koleksiyonunu alır. |
| [MinColumn](../../aspose.cells.gridweb.data/webcells/mincolumn/) { get; } | Veri veya stil içeren hücrenin minimum sütun numarası. |
| [MinRow](../../aspose.cells.gridweb.data/webcells/minrow/) { get; } | Veri veya stil içeren hücrenin minimum satır numarası. |
| [StandardHeight](../../aspose.cells.gridweb.data/webcells/standardheight/) { get; set; } | Bu çalışma sayfasındaki varsayılan satır yüksekliğini alır veya ayarlar, birim olarak puan. |
| [StandardWidth](../../aspose.cells.gridweb.data/webcells/standardwidth/) { get; set; } | Çalışma sayfasındaki varsayılan sütun genişliğini alır veya ayarlar, birim olarak karakter. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Clear](../../aspose.cells.gridweb.data/webcells/clear/)() |  |
| [ClearContents](../../aspose.cells.gridweb.data/webcells/clearcontents/)(int, int, int, int) | Bir aralığın içeriğini temizler. |
| [DeleteColumn](../../aspose.cells.gridweb.data/webcells/deletecolumn/)(int) | Bir sütunu siler. |
| [DeleteRow](../../aspose.cells.gridweb.data/webcells/deleterow/)(int) | Bir satırı siler. |
| [DeleteRows](../../aspose.cells.gridweb.data/webcells/deleterows/)(int, int) | Birçok satırı siler. Bu yöntem, toplu satır silme işlemi yaparken DeleteRow'dan çok daha hızlıdır. |
| [Export](../../aspose.cells.gridweb.data/webcells/export/)(int, int, int, int, bool, bool) | Bir WebWorksheet'in Cells koleksiyonundaki verileri yeni bir DataTable nesnesine dışa aktarır. |
| [ExportArray](../../aspose.cells.gridweb.data/webcells/exportarray/)(int, int, int, int) | Cells koleksiyonundaki verileri iki boyutlu dizi nesnesine dışa aktarır. |
| [GetColumnCaption](../../aspose.cells.gridweb.data/webcells/getcolumncaption/)(int) | Sütun başlığını alır. Başlık ayarlanmamışsa boş string döndürür. |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/webcells/getcolumnreadonly/)(int) | Bir sütunun yalnızca okunur olup olmadığını alır. Bu, GridWeb'e özgü genişletilmiş bir yöntemdir, gerçek Excel dosyasında tutulmaz ve etkili olmaz. |
| [GetColumnWidth](../../aspose.cells.gridweb.data/webcells/getcolumnwidth/)(int) | Belirtilen sütunun genişliğini alır |
| [GetEnumerator](../../aspose.cells.gridweb.data/webcells/getenumerator/)() | Hücre enumeratörünü alır. |
| [GetRowCaption](../../aspose.cells.gridweb.data/webcells/getrowcaption/)(int) | Satır başlığını alır. Başlık ayarlanmamışsa, boş dize döndürür. |
| [GetRowHeight](../../aspose.cells.gridweb.data/webcells/getrowheight/)(int) | Belirtilen bir satırın yüksekliğini alır. |
| [GetRowHiddenStatus](../../aspose.cells.gridweb.data/webcells/getrowhiddenstatus/)(int) | Belirtilen satırın gizli durumunu al. |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/webcells/getrowoutlinelevel/)(int) | Satırın anahat seviyesini alır. |
| [GetRowReadonly](../../aspose.cells.gridweb.data/webcells/getrowreadonly/)(int) | Bir satırın yalnızca okunur olup olmadığını alır. Bu, özellikle GridWeb'in genişletilmiş yöntemidir, gerçek Excel dosyasında korunmaz ve etkili olmaz. |
| [InsertColumn](../../aspose.cells.gridweb.data/webcells/insertcolumn/)(int) | Çalışma sayfasına yeni bir sütun ekler. |
| [InsertRow](../../aspose.cells.gridweb.data/webcells/insertrow/)(int) | Çalışma sayfasına yeni bir satır ekler. |
| [InsertRows](../../aspose.cells.gridweb.data/webcells/insertrows/)(int, int) | Çalışma sayfasına birden fazla satır ekler. |
| [Merge](../../aspose.cells.gridweb.data/webcells/merge/)(int, int, int, int) |  |
| [SetBorders](../../aspose.cells.gridweb.data/webcells/setborders/)(int, int, int, int, SetBorderPosition, WebBorderStyle) | Bir hücre aralığı için kenarlıkları ayarlar. |
| [SetColumnCaption](../../aspose.cells.gridweb.data/webcells/setcolumncaption/)(int, string) | Sütun için başlığı ayarlar. Lütfen bunun bir uzantı özelliği olduğunu ve Excel dosyasında korunamayacağını unutmayın. |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/webcells/setcolumnreadonly/)(int, bool) | Sütunu yalnızca okunur olarak ayarlar, böylece kullanıcı istemci tarafından silemez. Bu, özellikle GridWeb'in genişletilmiş yöntemidir ve gerçek Excel dosyasında korunmaz ve etkili olmaz. |
| [SetColumnWidth](../../aspose.cells.gridweb.data/webcells/setcolumnwidth/)(int, Unit) | Belirtilen sütunun genişliğini ayarlar. Kabul edilen genişlik türleri Point, Pixel veya Inch'tir. |
| [SetRowCaption](../../aspose.cells.gridweb.data/webcells/setrowcaption/)(int, string) | Satır için başlığı ayarlar. |
| [SetRowHeight](../../aspose.cells.gridweb.data/webcells/setrowheight/)(int, Unit) | Belirtilen satırın yüksekliğini ayarlar. Kabul edilen genişlik türleri Point, Pixel veya Inch'tir. |
| [SetRowHiddenStatus](../../aspose.cells.gridweb.data/webcells/setrowhiddenstatus/)(int, bool) | Belirtilen satırın gizli durumunu ayarlar. |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/webcells/setrowoutlinelevel/)(int, int) | Satırın anahat seviyesini ayarlar. |
| [SetRowOutlineLevelAndStatus](../../aspose.cells.gridweb.data/webcells/setrowoutlinelevelandstatus/)(int, int, bool) | Satırın anahat seviyesini ayarlar. |
| [SetRowReadonly](../../aspose.cells.gridweb.data/webcells/setrowreadonly/)(int, bool) | Satırı yalnızca okunur olarak ayarlar, böylece kullanıcı istemci tarafından silemez. Bu, özellikle GridWeb'in genişletilmiş yöntemidir ve gerçek Excel dosyasında korunmaz ve etkili olmaz. |
| [SetStyle](../../aspose.cells.gridweb.data/webcells/setstyle/#setstyle_1)(string, TableItemStyle) | Stili belirtilen hücre aralığına uygular. |
| [SetStyle](../../aspose.cells.gridweb.data/webcells/setstyle/#setstyle)(int, int, int, int, TableItemStyle) | Stili belirtilen hücre aralığına uygular. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort)(int, int, int, int, int) | WebWorksheet aralığında belirtilen sütun indeksine göre verileri yukarıdan aşağıya artan şekilde sıralar. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_2)(int, int, int, int, int[]) | WebWorksheet aralığında, sütun indeksleri dizisiyle belirtilen bazı alanlara göre verileri yukarıdan aşağıya artan şekilde sıralar. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_1)(int, int, int, int, int, SortByOrder, SortOrientation, bool) | WebWorksheet aralığında belirtilen sütun indeksine göre verileri yukarıdan aşağıya artan şekilde sıralar. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_3)(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) | WebWorksheet aralığında, indeks dizisiyle belirtilen bazı alanlara göre verileri artan şekilde sıralar. |
| [UnMerge](../../aspose.cells.gridweb.data/webcells/unmerge/)(int, int, int, int) | Belirtilen birleştirilmiş hücre aralığının birleştirmesini kaldırır. |
| static [CellIndexToName](../../aspose.cells.gridweb.data/webcells/cellindextoname/)(int, int) | Satır ve sütun indekslerine göre hücre adını alır. |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/webcells/cellnametoindex/)(string, out int, out int) | Hücrenin adını temel alarak satır ve sütun indekslerini alır. |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/webcells/columnindextoname/)(int) | Sütun indeksine göre sütun adını alır. |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/webcells/columnnametoindex/)(string) | Sütun adına göre sütun indeksini alır. |

### Açıklamalar

NOT: Bu sınıf artık kullanımdan kaldırılmıştır. Lütfen bunun yerine GridCells kullanın. Bu sınıf, Ağustos 2014'ten itibaren 6 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


