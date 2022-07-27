---
title: Cells
second_title: Aspose.Cells for .NET API Referansı
description: Aşağıdakiler gibi hücreyle ilgili nesnelerin bir koleksiyonunu kapsüllerCell./cell Row./row ...etc.
type: docs
weight: 300
url: /tr/net/aspose.cells/cells/
---
## Cells class

Aşağıdakiler gibi hücreyle ilgili nesnelerin bir koleksiyonunu kapsüller:[`Cell`](../cell) ,[`Row`](../row) ...etc.

```csharp
public class Cells : IDisposable, IEnumerable
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [Columns](../../aspose.cells/cells/columns) { get; } | Şunların koleksiyonunu alır:[`Column`](../column) bu çalışma sayfasındaki tek tek sütunları temsil eden nesneler. |
| [Count](../../aspose.cells/cells/count) { get; } | Örneklenen Cell nesnelerinin toplam sayısını alır. |
| [CountLarge](../../aspose.cells/cells/countlarge) { get; } | Örneklenen Cell nesnelerinin toplam sayısını alır. |
| [FirstCell](../../aspose.cells/cells/firstcell) { get; } | Bu çalışma sayfasındaki ilk hücreyi alır. |
| [IsDefaultRowHeightMatched](../../aspose.cells/cells/isdefaultrowheightmatched) { get; set; } | Satır yüksekliği ile varsayılan yazı tipi yüksekliğinin eşleştiğini gösterir |
| [IsDefaultRowHidden](../../aspose.cells/cells/isdefaultrowhidden) { get; set; } | Satırın varsayılan olarak gizli olup olmadığını gösterir. |
| [Item](../../aspose.cells/cells/item) { get; } | [`Cell`](../cell) belirtilen hücre satırı dizini ve sütun dizinindeki öğe. (2 indexers) |
| [LastCell](../../aspose.cells/cells/lastcell) { get; } | Bu çalışma sayfasındaki son hücreyi alır. |
| [MaxColumn](../../aspose.cells/cells/maxcolumn) { get; } | Koleksiyonda somutlaştırılan bu hücrelerin minimum sütun dizini (sütun 'yi içermez, burada stil tüm sütun için tanımlanır, ancak içinde hiçbir hücre somutlaştırılmaz). |
| [MaxDataColumn](../../aspose.cells/cells/maxdatacolumn) { get; } | Veri içeren hücrenin maksimum sütun dizini. |
| [MaxDataRow](../../aspose.cells/cells/maxdatarow) { get; } | Veri içeren hücrenin maksimum satır dizini. |
| [MaxDisplayRange](../../aspose.cells/cells/maxdisplayrange) { get; } | Verileri, birleştirilmiş hücreleri ve şekilleri içeren maksimum aralığı alır. |
| [MaxRow](../../aspose.cells/cells/maxrow) { get; } | Veri veya stil içeren hücrenin maksimum satır dizini. |
| [MemorySetting](../../aspose.cells/cells/memorysetting) { get; set; } | Bu hücreler için bellek kullanımı seçeneğini alır veya ayarlar. |
| [MergedCells](../../aspose.cells/cells/mergedcells) { get; } | Birleştirilmiş hücrelerin koleksiyonunu alır. |
| [MinColumn](../../aspose.cells/cells/mincolumn) { get; } | Koleksiyonda somutlaştırılan bu hücrelerin minimum sütun dizini (sütun 'yi içermez, burada stil tüm sütun için tanımlanır, ancak içinde hiçbir hücre somutlaştırılmaz). |
| [MinDataColumn](../../aspose.cells/cells/mindatacolumn) { get; } | Veri içeren hücrenin minimum sütun dizini. |
| [MinDataRow](../../aspose.cells/cells/mindatarow) { get; } | Veri içeren hücrenin minimum satır dizini. |
| [MinRow](../../aspose.cells/cells/minrow) { get; } | Veri veya stil içeren hücrenin minimum satır dizini. |
| [MultiThreadReading](../../aspose.cells/cells/multithreadreading) { get; set; } | Hücre veri modelinin Çoklu İş parçacığı okumayı destekleyip desteklemediğini alır veya ayarlar. Bu özelliğin varsayılan değeri false'tur. |
| [OdsCellFields](../../aspose.cells/cells/odscellfields) { get; } | ods. alanlarının listesini alır |
| [PreserveString](../../aspose.cells/cells/preservestring) { get; set; } | Tüm çalışma sayfası değerlerinin dize olarak korunup korunmadığını belirten bir değer alır veya ayarlar. Varsayılan yanlıştır. |
| [Ranges](../../aspose.cells/cells/ranges) { get; } | Şunların koleksiyonunu alır:[`Range`](../range)çalışma zamanında oluşturulan nesneler. |
| [Rows](../../aspose.cells/cells/rows) { get; } | Şunların koleksiyonunu alır:[`Row`](../row) bu çalışma sayfasındaki tek tek satırları temsil eden nesneler. |
| [StandardHeight](../../aspose.cells/cells/standardheight) { get; set; } | Bu çalışma sayfasındaki varsayılan satır yüksekliğini puan birimi olarak alır veya ayarlar. |
| [StandardHeightInch](../../aspose.cells/cells/standardheightinch) { get; set; } | Bu çalışma sayfasındaki varsayılan satır yüksekliğini inç cinsinden alır veya ayarlar. |
| [StandardHeightPixels](../../aspose.cells/cells/standardheightpixels) { get; set; } | Bu çalışma sayfasındaki varsayılan satır yüksekliğini piksel birimi olarak alır veya ayarlar. |
| [StandardWidth](../../aspose.cells/cells/standardwidth) { get; set; } | Çalışma sayfasındaki varsayılan sütun genişliğini karakter birimi cinsinden alır veya ayarlar. |
| [StandardWidthInch](../../aspose.cells/cells/standardwidthinch) { get; set; } | Çalışma sayfasındaki varsayılan sütun genişliğini inç cinsinden alır veya ayarlar. |
| [StandardWidthPixels](../../aspose.cells/cells/standardwidthpixels) { get; set; } | Çalışma sayfasındaki varsayılan sütun genişliğini piksel birimi olarak alır veya ayarlar. |
| [Style](../../aspose.cells/cells/style) { get; set; } | Varsayılan stili alır ve ayarlar. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [AddRange](../../aspose.cells/cells/addrange)(Range) | cell öğesine bir aralık nesnesi başvurusu ekler |
| [ApplyColumnStyle](../../aspose.cells/cells/applycolumnstyle)(int, Style, StyleFlag) | Tüm sütun için biçimleri uygular. |
| [ApplyRowStyle](../../aspose.cells/cells/applyrowstyle)(int, Style, StyleFlag) | Tüm satır için biçimleri uygular. |
| [ApplyStyle](../../aspose.cells/cells/applystyle)(Style, StyleFlag) | Tüm çalışma sayfası için biçimleri uygular. |
| [CheckCell](../../aspose.cells/cells/checkcell)(int, int) | [`Cell`](../cell) belirtilen hücre satırı dizininde ve sütun dizininde öğe veya null. |
| [CheckColumn](../../aspose.cells/cells/checkcolumn)(int) | [`Column`](../column) belirtilen sütun dizininde öğe veya null. |
| [CheckRow](../../aspose.cells/cells/checkrow)(int) | [`Row`](../row) öğede veya belirtilen hücre satırı dizininde. |
| [Clear](../../aspose.cells/cells/clear)() | Tüm hücre ve satır nesnelerini temizler. |
| [ClearContents](../../aspose.cells/cells/clearcontents#clearcontents)(CellArea) | Bir aralığın içeriğini temizler. |
| [ClearContents](../../aspose.cells/cells/clearcontents#clearcontents_1)(int, int, int, int) | Bir aralığın içeriğini temizler. |
| [ClearFormats](../../aspose.cells/cells/clearformats#clearformats)(CellArea) | Bir aralığın biçimlendirmesini temizler. |
| [ClearFormats](../../aspose.cells/cells/clearformats#clearformats_1)(int, int, int, int) | Bir aralığın biçimlendirmesini temizler. |
| [ClearMergedCells](../../aspose.cells/cells/clearmergedcells)() | Birleştirilmiş tüm aralıkları temizler. |
| [ClearRange](../../aspose.cells/cells/clearrange#clearrange)(CellArea) | Bir aralığın içeriğini ve biçimlendirmesini temizler. |
| [ClearRange](../../aspose.cells/cells/clearrange#clearrange_1)(int, int, int, int) | Bir aralığın içeriğini ve biçimlendirmesini temizler. |
| [ConvertStringToNumericValue](../../aspose.cells/cells/convertstringtonumericvalue)() | Mümkünse hücrelerdeki dize verilerini sayısal değere dönüştürür. |
| [CopyColumn](../../aspose.cells/cells/copycolumn)(Cells, int, int) | Tüm sütunun verilerini ve biçimlerini kopyalar. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns)(Cells, int, int, int) | Tüm sütunun verilerini ve biçimlerini kopyalar. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns_2)(Cells, int, int, int, int) | Tüm sütunların verilerini ve biçimlerini kopyalar. |
| [CopyColumns](../../aspose.cells/cells/copycolumns#copycolumns_1)(Cells, int, int, int, PasteOptions) | Tüm sütunun verilerini ve biçimlerini kopyalar. |
| [CopyRow](../../aspose.cells/cells/copyrow)(Cells, int, int) | Tüm satırın verilerini ve biçimlerini kopyalar. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows)(Cells, int, int, int) | Bazı tüm satırların verilerini ve biçimlerini kopyalar. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows_1)(Cells, int, int, int, CopyOptions) | Bazı tüm satırların verilerini ve biçimlerini kopyalar. |
| [CopyRows](../../aspose.cells/cells/copyrows#copyrows_2)(Cells, int, int, int, CopyOptions, PasteOptions) | Bazı tüm satırların verilerini ve biçimlerini kopyalar. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_2)(string) | Bir[`Range`](../range) aralığının bir adresinden nesne. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_3)(string, string) | Bir[`Range`](../range) bir hücre aralığından nesne. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange)(int, int, bool) | Bir[`Range`](../range) hücre satırlarından veya hücre sütunlarından nesne. |
| [CreateRange](../../aspose.cells/cells/createrange#createrange_1)(int, int, int, int) | Bir[`Range`](../range) bir hücre aralığından nesne. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns#deleteblankcolumns)() | Herhangi bir veri içermeyen tüm boş sütunları silin. |
| [DeleteBlankColumns](../../aspose.cells/cells/deleteblankcolumns#deleteblankcolumns_1)(DeleteOptions) | Herhangi bir veri içermeyen tüm boş sütunları silin. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows#deleteblankrows)() | Herhangi bir veri içermeyen tüm boş satırları silin. |
| [DeleteBlankRows](../../aspose.cells/cells/deleteblankrows#deleteblankrows_1)(DeleteOptions) | Herhangi bir veri içermeyen tüm boş satırları silin. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn#deletecolumn)(int) | Bir sütunu siler. |
| [DeleteColumn](../../aspose.cells/cells/deletecolumn#deletecolumn_1)(int, bool) | Bir sütunu siler. |
| [DeleteColumns](../../aspose.cells/cells/deletecolumns)(int, int, bool) | Birkaç sütunu siler. |
| [DeleteRange](../../aspose.cells/cells/deleterange)(int, int, int, int, ShiftType) | Bir hücre aralığını siler ve kaydırma seçeneğine göre hücreleri kaydırır. |
| [DeleteRow](../../aspose.cells/cells/deleterow)(int) | Bir satırı siler. |
| [DeleteRows](../../aspose.cells/cells/deleterows#deleterows)(int, int) | Birkaç satırı siler. |
| [DeleteRows](../../aspose.cells/cells/deleterows#deleterows_1)(int, int, bool) | Çalışma sayfasındaki birden çok satırı siler. |
| [Dispose](../../aspose.cells/cells/dispose)() | Yönetilmeyen kaynakları serbest bırakma, serbest bırakma veya sıfırlama ile ilişkili uygulama tanımlı görevleri gerçekleştirir. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn#endcellincolumn)(short) | Bu sütundaki son hücreyi alır. |
| [EndCellInColumn](../../aspose.cells/cells/endcellincolumn#endcellincolumn_1)(int, int, short, short) | Bu aralıktaki maksimum sütun indeksine sahip son hücreyi alır. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow#endcellinrow)(int) | Bu satırdaki son hücreyi alır. |
| [EndCellInRow](../../aspose.cells/cells/endcellinrow#endcellinrow_1)(int, int, int, int) | Bu aralıktaki maksimum satır indeksine sahip son hücreyi alır. |
| [ExportArray](../../aspose.cells/cells/exportarray)(int, int, int, int) | Verileri şurada dışa aktarır:[`Cells`](../cells) iki boyutlu bir dizi nesnesine toplama. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable)(int, int, int, int) | Verileri şurada dışa aktarır:[`Cells`](../cells) toplama birDataTable nesne. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable_2)(int, int, int, int, bool) | Verileri şurada dışa aktarır:[`Cells`](../cells) toplama birDataTable nesne. |
| [ExportDataTable](../../aspose.cells/cells/exportdatatable#exportdatatable_1)(int, int, int, int, ExportTableOptions) | Verileri şurada dışa aktarır:[`Cells`](../cells) toplama birDataTable nesne. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring#exportdatatableasstring)(int, int, int, int) | Verileri şurada dışa aktarır:[`Cells`](../cells) toplama birDataTable nesne. |
| [ExportDataTableAsString](../../aspose.cells/cells/exportdatatableasstring#exportdatatableasstring_1)(int, int, int, int, bool) | Verileri şurada dışa aktarır:[`Cells`](../cells) toplama birDataTable nesne. |
| [ExportTypeArray](../../aspose.cells/cells/exporttypearray)(int, int, int, int) | [`Cells`](../cells) iki boyutlu bir dizi nesnesine toplama. |
| [Find](../../aspose.cells/cells/find#find)(object, Cell) | Girdi nesnesini içeren hücreyi bulur. |
| [Find](../../aspose.cells/cells/find#find_1)(object, Cell, FindOptions) | Girdi nesnesini içeren hücreyi bulur. |
| [GetCell](../../aspose.cells/cells/getcell)(int, int) | [`Cell`](../cell) belirtilen hücre satırı dizininde ve sütun dizininde öğe veya null. |
| [GetCellStyle](../../aspose.cells/cells/getcellstyle)(int, int) | Verilen hücrenin stilini alın. |
| [GetColumnWidth](../../aspose.cells/cells/getcolumnwidth)(int) | Normal görünümde belirtilen sütunun genişliğini alır |
| [GetColumnWidthInch](../../aspose.cells/cells/getcolumnwidthinch)(int) | Normal görünümde belirtilen sütunun genişliğini inç cinsinden alır. |
| [GetColumnWidthPixel](../../aspose.cells/cells/getcolumnwidthpixel)(int) | Normal görünümde belirtilen sütunun genişliğini piksel birimi cinsinden alır. |
| [GetDependents](../../aspose.cells/cells/getdependents)(bool, int, int) | Belirli hücreye başvuran tüm hücreleri alın. |
| [GetDependentsInCalculation](../../aspose.cells/cells/getdependentsincalculation)(int, int, bool) | Hesaplanan sonucu belirli hücreye bağlı olan tüm hücreleri alır. |
| [GetEnumerator](../../aspose.cells/cells/getenumerator)() | Hücre numaralandırıcısını alır. |
| [GetGroupedColumnOutlineLevel](../../aspose.cells/cells/getgroupedcolumnoutlinelevel)(int) | Sütunun anahat düzeyini (sıfır tabanlı) alır. |
| [GetGroupedRowOutlineLevel](../../aspose.cells/cells/getgroupedrowoutlinelevel)(int) | Satırın anahat düzeyini (sıfır tabanlı) alır. |
| [GetLastDataRow](../../aspose.cells/cells/getlastdatarow)(int) | Belirtilen sütundaki verileri içeren hücrenin son satır dizinini alır. |
| [GetMaxGroupedColumnOutlineLevel](../../aspose.cells/cells/getmaxgroupedcolumnoutlinelevel)() | Maksimum gruplandırılmış sütun anahat düzeyini alır (sıfır tabanlı). |
| [GetMaxGroupedRowOutlineLevel](../../aspose.cells/cells/getmaxgroupedrowoutlinelevel)() | Maksimum gruplandırılmış satır anahat düzeyini alır (sıfır tabanlı). |
| [GetRow](../../aspose.cells/cells/getrow)(int) | [`Row`](../row) belirtilen hücre satırı dizinindeki öğe. |
| [GetRowEnumerator](../../aspose.cells/cells/getrowenumerator)() | Satır numaralandırıcısını alır. |
| [GetRowHeight](../../aspose.cells/cells/getrowheight)(int) | Belirtilen satırın yüksekliğini alır. |
| [GetRowHeightInch](../../aspose.cells/cells/getrowheightinch)(int) | Belirtilen satırın yüksekliğini inç cinsinden alır. |
| [GetRowHeightPixel](../../aspose.cells/cells/getrowheightpixel)(int) | Belirtilen satırın yüksekliğini piksel birimi cinsinden alır. |
| [GetRowOriginalHeightPoint](../../aspose.cells/cells/getroworiginalheightpoint)(int) | Satır gizliyse, orijinal satırın yüksekliğini nokta birimi cinsinden alır |
| [GetViewColumnWidthPixel](../../aspose.cells/cells/getviewcolumnwidthpixel)(int) | Genişliği farklı görünüm türünde alın. |
| [GetViewRowHeight](../../aspose.cells/cells/getviewrowheight)(int) | Belirtilen satırın yüksekliğini alır. |
| [GetViewRowHeightInch](../../aspose.cells/cells/getviewrowheightinch)(int) | Belirtilen satırın yüksekliğini inç cinsinden alır. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns#groupcolumns)(int, int) | Grup sütunları. |
| [GroupColumns](../../aspose.cells/cells/groupcolumns#groupcolumns_1)(int, int, bool) | Grup sütunları. |
| [GroupRows](../../aspose.cells/cells/grouprows#grouprows)(int, int) | Grup satırları. |
| [GroupRows](../../aspose.cells/cells/grouprows#grouprows_1)(int, int, bool) | Grup satırları. |
| [HideColumn](../../aspose.cells/cells/hidecolumn)(int) | Bir sütunu gizler. |
| [HideColumns](../../aspose.cells/cells/hidecolumns)(int, int) | Birden çok sütunu gizleyin. |
| [HideGroupDetail](../../aspose.cells/cells/hidegroupdetail)(bool, int) | Gruplandırılmış satırları/sütunları daraltır. |
| [HideRow](../../aspose.cells/cells/hiderow)(int) | Bir satırı gizler. |
| [HideRows](../../aspose.cells/cells/hiderows)(int, int) | Birden çok satırı gizler. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray)(double[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_2)(int[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_4)(string[], int, int) |  |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_1)(double[], int, int, bool) | Double dizisini bir çalışma sayfasına aktarır. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_3)(int[], int, int, bool) | Bir tamsayı dizisini bir çalışma sayfasına aktarır. |
| [ImportArray](../../aspose.cells/cells/importarray#importarray_5)(string[], int, int, bool) | Bir dize dizisini bir çalışma sayfasına aktarır. |
| [ImportArrayList](../../aspose.cells/cells/importarraylist)(ArrayList, int, int, bool) | Bir dizi veri listesini bir çalışma sayfasına aktarır. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv)(Stream, TxtLoadOptions, int, int) | Hücrelere bir CSV dosyası aktarın. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_2)(string, TxtLoadOptions, int, int) | Hücrelere bir CSV dosyası aktarın. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_1)(Stream, string, bool, int, int) | Hücrelere bir CSV dosyası aktarın. |
| [ImportCSV](../../aspose.cells/cells/importcsv#importcsv_3)(string, string, bool, int, int) | Hücrelere bir CSV dosyası aktarın. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects#importcustomobjects)(ICollection, int, int, ImportTableOptions) | Özel nesneleri içe aktarır. |
| [ImportCustomObjects](../../aspose.cells/cells/importcustomobjects#importcustomobjects_1)(ICollection, string[], bool, int, int, int, bool, string, bool) | Özel nesneleri içe aktarır. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_3)(IDataReader, int, int) | Verileri birIDataReader nesne. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_1)(DataTable, int, int, ImportTableOptions) | Özel veri tablosundan verileri içe aktarın. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_2)(DataView, int, int, ImportTableOptions) | Veri görünümünden verileri içe aktarın. |
| [ImportData](../../aspose.cells/cells/importdata#importdata)(ICellsDataTable, int, int, ImportTableOptions) | Özel veri tablosundan verileri içe aktarın. |
| [ImportData](../../aspose.cells/cells/importdata#importdata_4)(IDataReader, int, int, ImportTableOptions) | Verileri birIDataReader nesne. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid)(DataGrid, int, int, bool) | BirDataGrid bir çalışma sayfasına. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid_1)(DataGrid, int, int, int, int, bool) | BirDataGrid bir çalışma sayfasına. |
| [ImportDataGrid](../../aspose.cells/cells/importdatagrid#importdatagrid_2)(DataGrid, int, int, int, int, bool, bool) | BirDataGrid bir çalışma sayfasına. |
| [ImportDataGridAsString](../../aspose.cells/cells/importdatagridasstring)(DataGrid, int, int, bool) | BirDataGrid bir çalışma sayfasına dönüştürün. Bu yöntem, metni sayısal değerlere dönüştürmeye çalışmaz. |
| [ImportDataRow](../../aspose.cells/cells/importdatarow)(DataRow, int, int) | Bir DataRow'u Excel dosyasına aktarır. |
| [ImportDataView](../../aspose.cells/cells/importdataview#importdataview_3)(DataView, int, int) | BirDataView bir çalışma sayfasına. |
| [ImportFormulaArray](../../aspose.cells/cells/importformulaarray)(string[], int, int, bool) | Bir formül dizisini çalışma sayfasına aktarır. |
| [ImportGridView](../../aspose.cells/cells/importgridview)(GridView, int, int, ImportTableOptions) | Bu hücrelere bir ızgara görünümü aktarır. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray#importobjectarray)(object[], int, int, bool) | Bir dizi veriyi bir çalışma sayfasına aktarır. |
| [ImportObjectArray](../../aspose.cells/cells/importobjectarray#importobjectarray_1)(object[], int, int, bool, int) | Bir dizi veriyi bir çalışma sayfasına aktarır. |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray)(object[], int, int) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_1)(object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_3)(object[], object[], int, int, bool) |  |
| [ImportTwoDimensionArray](../../aspose.cells/cells/importtwodimensionarray#importtwodimensionarray_2)(object[], object[], int, int, TxtLoadOptions) |  |
| [InsertColumn](../../aspose.cells/cells/insertcolumn#insertcolumn)(int) | Çalışma sayfasına yeni bir sütun ekler. |
| [InsertColumn](../../aspose.cells/cells/insertcolumn#insertcolumn_1)(int, bool) | Çalışma sayfasına yeni bir sütun ekler. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns#insertcolumns)(int, int) | Çalışma sayfasına bazı sütunlar ekler. |
| [InsertColumns](../../aspose.cells/cells/insertcolumns#insertcolumns_1)(int, int, bool) | Çalışma sayfasına bazı sütunlar ekler. |
| [InsertCutCells](../../aspose.cells/cells/insertcutcells)(Range, int, int, ShiftType) | Kesim aralığını ekleyin. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange)(CellArea, ShiftType) | Bir hücre aralığı ekler ve hücreleri kaydırma seçeneğine göre kaydırır. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange_1)(CellArea, int, ShiftType) | Bir hücre aralığı ekler ve hücreleri kaydırma seçeneğine göre kaydırır. |
| [InsertRange](../../aspose.cells/cells/insertrange#insertrange_2)(CellArea, int, ShiftType, bool) | Bir hücre aralığı ekler ve hücreleri kaydırma seçeneğine göre kaydırır. |
| [InsertRow](../../aspose.cells/cells/insertrow)(int) | Çalışma sayfasına yeni bir satır ekler. |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows)(int, int) | Çalışma sayfasına birden çok satır ekler. |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows_2)(int, int, bool) | Çalışma sayfasına birden çok satır ekler. |
| [InsertRows](../../aspose.cells/cells/insertrows#insertrows_1)(int, int, InsertOptions) | Çalışma sayfasına birden çok satır ekler. |
| [IsBlankColumn](../../aspose.cells/cells/isblankcolumn)(int) | Verilen sütunun boş olup olmadığını kontrol eder (hiçbir veri içermez). |
| [IsColumnHidden](../../aspose.cells/cells/iscolumnhidden)(int) | Verilen dizindeki bir sütunun gizli olup olmadığını kontrol eder. |
| [IsDeletingRangeEnabled](../../aspose.cells/cells/isdeletingrangeenabled)(int, int, int, int) | Aralığın silinip silinemeyeceğini kontrol edin. |
| [IsRowHidden](../../aspose.cells/cells/isrowhidden)(int) | Verilen dizindeki bir satırın gizli olup olmadığını kontrol eder. |
| [LinkToXmlMap](../../aspose.cells/cells/linktoxmlmap)(string, int, int, string) | Bir xml haritasına bağlantı. |
| [Merge](../../aspose.cells/cells/merge#merge)(int, int, int, int) | Belirtilen hücre aralığını tek bir hücrede birleştirir. |
| [Merge](../../aspose.cells/cells/merge#merge_1)(int, int, int, int, bool) | Belirtilen hücre aralığını tek bir hücrede birleştirir. |
| [Merge](../../aspose.cells/cells/merge#merge_2)(int, int, int, int, bool, bool) | Belirtilen hücre aralığını tek bir hücrede birleştirir. |
| [MoveRange](../../aspose.cells/cells/moverange)(CellArea, int, int) | Aralığı hareket ettirir. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates)() | Sayfadaki yinelenen satırları kaldırır. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates_1)(int, int, int, int) | Aralıktaki yinelenen değerleri kaldırır. |
| [RemoveDuplicates](../../aspose.cells/cells/removeduplicates#removeduplicates_2)(int, int, int, int, bool, int[]) | Aralığın yinelenen verilerini kaldırır. |
| [RemoveFormulas](../../aspose.cells/cells/removeformulas)() | Tüm formülü kaldırır ve formülün değeriyle değiştirir. |
| [RetrieveSubtotalSetting](../../aspose.cells/cells/retrievesubtotalsetting)(CellArea) | Aralığın alt toplamları ayarını alır. |
| [SetColumnWidth](../../aspose.cells/cells/setcolumnwidth)(int, double) | Normal görünümde belirtilen sütunun genişliğini ayarlar. |
| [SetColumnWidthInch](../../aspose.cells/cells/setcolumnwidthinch)(int, double) | Normal görünümde sütun genişliğini inç cinsinden ayarlar. |
| [SetColumnWidthPixel](../../aspose.cells/cells/setcolumnwidthpixel)(int, int) | Normal görünümde sütun genişliğini piksel birimi olarak ayarlar. |
| [SetRowHeight](../../aspose.cells/cells/setrowheight)(int, double) | Belirtilen satırın yüksekliğini ayarlar. |
| [SetRowHeightInch](../../aspose.cells/cells/setrowheightinch)(int, double) | Satır yüksekliğini inç cinsinden ayarlar. |
| [SetRowHeightPixel](../../aspose.cells/cells/setrowheightpixel)(int, int) | Satır yüksekliğini piksel birimi olarak ayarlar. |
| [SetViewColumnWidthPixel](../../aspose.cells/cells/setviewcolumnwidthpixel)(int, int) | Farklı görünümde sütunun genişliğini ayarlar. |
| [ShowGroupDetail](../../aspose.cells/cells/showgroupdetail)(bool, int) | Gruplandırılmış satırları/sütunları genişletir. |
| [Subtotal](../../aspose.cells/cells/subtotal#subtotal)(CellArea, int, ConsolidationFunction, int[]) | Aralık için alt toplamlar oluşturur. |
| [Subtotal](../../aspose.cells/cells/subtotal#subtotal_1)(CellArea, int, ConsolidationFunction, int[], bool, bool, bool) | Aralık için alt toplamlar oluşturur. |
| [TextToColumns](../../aspose.cells/cells/texttocolumns)(int, int, int, TxtLoadOptions) | Sütundaki metni sütunlara böler. |
| [UngroupColumns](../../aspose.cells/cells/ungroupcolumns)(int, int) | Sütunların grubunu çözer. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows#ungrouprows)(int, int) | Satırların grubunu çözer. |
| [UngroupRows](../../aspose.cells/cells/ungrouprows#ungrouprows_1)(int, int, bool) | Satırların grubunu çözer. |
| [UnhideColumn](../../aspose.cells/cells/unhidecolumn)(int, double) | Bir sütunu gösterir |
| [UnhideColumns](../../aspose.cells/cells/unhidecolumns)(int, int, double) | Birden çok sütunu göster. |
| [UnhideRow](../../aspose.cells/cells/unhiderow)(int, double) | Bir satırı gösterir. |
| [UnhideRows](../../aspose.cells/cells/unhiderows)(int, int, double) | Gizli satırları gösterir. |
| [UnMerge](../../aspose.cells/cells/unmerge)(int, int, int, int) | Belirtilen birleştirilmiş hücre aralığını kaldırır. |

### Örnekler

```csharp

[C#]

Workbook excel = new Workbook();
Cells cells = excel.Worksheets[0].Cells;

// Varsayılan satır yüksekliğini ayarla
cells.StandardHeight = 20;
// Satır yüksekliğini ayarla
cells.SetRowHeight(2, 20.5);

// Varsayılan sütun genişliğini ayarla
cells.StandardWidth = 15;
// Sütun genişliğini ayarla
cells.SetColumnWidth(3, 12.57);

//Hücreleri birleştir
cells.Merge(5, 4, 2, 2);

//Hücrelere değer koy
cells[0, 0].PutValue(true);
cells[0, 1].PutValue(1);
cells[0, 2].PutValue("abc");

//Verileri dışa aktar
object[,] arr = cells.ExportArray(0, 0, 10, 10);

[Visual Basic]

Dim excel as Workbook = new Workbook()
Dim cells as Cells = excel.Worksheets(0).Cells

'Varsayılan satır yüksekliğini ayarla
cells.StandardHeight = 20
'Satır yüksekliğini ayarla
cells.SetRowHeight(2, 20.5)

'Varsayılan sütun genişliğini ayarla
cells.StandardWidth = 15
'Sütun genişliğini ayarla
cells.SetColumnWidth(3, 12.57)

'Hücreleri birleştir
cells.Merge(5, 4, 2, 2)

'Verileri dışa aktar
Dim outDataTable as DataTable = cells.ExportDataTable(12, 12, 10, 10)
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
