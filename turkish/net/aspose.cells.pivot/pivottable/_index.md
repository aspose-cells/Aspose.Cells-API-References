---
title: "Sınıf PivotTable"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Pivot.PivotTable sınıfı. PivotTable için özet açıklama"
type: docs
url: /tr/net/aspose.cells.pivot/pivottable/
---
## PivotTable class

PivotTable için özet açıklama.

```csharp
public class PivotTable : IDisposable
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AllowMultipleFiltersPerField](../../aspose.cells.pivot/pivottable/allowmultiplefiltersperfield/) { get; set; } | PivotTable alanlarının birden fazla filtreye sahip olup olamayacağını belirten bir boolean değer belirtir. |
| [AltTextDescription](../../aspose.cells.pivot/pivottable/alttextdescription/) { get; set; } | Alt metnin açıklamasını alır. |
| [AltTextTitle](../../aspose.cells.pivot/pivottable/alttexttitle/) { get; set; } | Alternatif metnin başlığını alır ve ayarlar. |
| [AutofitColumnWidthOnUpdate](../../aspose.cells.pivot/pivottable/autofitcolumnwidthonupdate/) { get; set; } | Güncelleme sırasında sütun genişliğinin otomatik olarak ayarlanıp ayarlanmayacağını belirtir. |
| [AutoFormatType](../../aspose.cells.pivot/pivottable/autoformattype/) { get; set; } | PivotTable'ın otomatik biçim türünü alır ve ayarlar. |
| [BaseFields](../../aspose.cells.pivot/pivottable/basefields/) { get; } | PivotTable içindeki tüm temel pivot alanlarını döndürür. |
| [ColumnFields](../../aspose.cells.pivot/pivottable/columnfields/) { get; } | Şu anda sütun alanları olarak gösterilen bir PivotFields nesnesini döndürür. |
| [ColumnGrand](../../aspose.cells.pivot/pivottable/columngrand/) { get; set; } | (**Eski.**) PivotTable raporunun sütunlar için genel toplamları gösterip göstermediğini belirtir. |
| [ColumnHeaderCaption](../../aspose.cells.pivot/pivottable/columnheadercaption/) { get; set; } | PivotTable'ın sütun başlığının özel başlığını alır ve ayarlar. |
| [ColumnRange](../../aspose.cells.pivot/pivottable/columnrange/) { get; } | PivotTable raporundaki sütun alanını içeren aralığı temsil eden bir CellArea nesnesini döndürür. Yalnızca okunabilir. |
| [ConditionalFormats](../../aspose.cells.pivot/pivottable/conditionalformats/) { get; } | Pivot tablonun koşullu biçimlendirmelerini alır. |
| [CustomListSort](../../aspose.cells.pivot/pivottable/customlistsort/) { get; set; } | Veri sıralanırken yerleşik özel listenin dikkate alınıp alınmayacağını belirtir. |
| [DataBodyRange](../../aspose.cells.pivot/pivottable/databodyrange/) { get; } | Başlık satırı ile ek satır arasındaki listedeki veri alanını içeren aralığı temsil eden bir [`CellArea`](../../aspose.cells/cellarea/) nesnesini döndürür. Yalnızca okunabilir. |
| [DataField](../../aspose.cells.pivot/pivottable/datafield/) { get; } | (**Eski.**) Bir PivotTable'daki tüm veri alanlarını temsil eden bir [`PivotField`](../pivotfield/) nesnesini alır. Yalnızca okunabilir. Veri bölgesinde iki veya daha fazla veri alanı olduğunda oluşturulur. Varsayılan olarak satır bölgesindedir. PivotTable.AddFieldToArea() yöntemiyle satır/sütun bölgesine sürükleyebilirsiniz. |
| [DataFieldHeaderName](../../aspose.cells.pivot/pivottable/datafieldheadername/) { get; set; } | PivotTable'daki değer alanı başlığının adını alır ve ayarlar. |
| [DataFields](../../aspose.cells.pivot/pivottable/datafields/) { get; } | Bir PivotTable'daki tüm veri alanlarını temsil eden bir [`PivotFieldCollection`](../pivotfieldcollection/) alır. |
| [DataSource](../../aspose.cells.pivot/pivottable/datasource/) { get; set; } | Pivot tablonun veri kaynağını alır ve ayarlar. |
| [DisplayErrorString](../../aspose.cells.pivot/pivottable/displayerrorstring/) { get; set; } | PivotTable raporunun hata içeren hücrelerde özel bir metin gösterip göstermediğini belirtir. |
| [DisplayImmediateItems](../../aspose.cells.pivot/pivottable/displayimmediateitems/) { get; set; } | PivotTable'ın veri alanı boş olduğunda satır ve sütun bölgelerindeki öğelerin görünür olup olmadığını belirtir. Varsayılan değer doğrudur. |
| [DisplayNullString](../../aspose.cells.pivot/pivottable/displaynullstring/) { get; set; } | PivotTable raporunun değer null olduğunda özel bir metin gösterip göstermediğini belirtir. |
| [EnableDataValueEditing](../../aspose.cells.pivot/pivottable/enabledatavalueediting/) { get; set; } | Kullanıcının pivottable veri alanındaki hücreleri düzenlemesine izin verilip verilmediğini belirten bir boolean değer belirtir. Varsayılan değer yanlıştır. |
| [EnableDrilldown](../../aspose.cells.pivot/pivottable/enabledrilldown/) { get; set; } | Ayrıntıya inmenin etkin olup olmadığını belirtir. |
| [EnableFieldDialog](../../aspose.cells.pivot/pivottable/enablefielddialog/) { get; set; } | Kullanıcı PivotTable alanına çift tıkladığında PivotTable Field iletişim kutusunun mevcut olup olmadığını gösterir. |
| [EnableFieldList](../../aspose.cells.pivot/pivottable/enablefieldlist/) { get; set; } | Excel görünümünde **PivotTable** için alan listesinin mevcut olup olmadığını gösterir. |
| [EnableWizard](../../aspose.cells.pivot/pivottable/enablewizard/) { get; set; } | **PivotTable Wizard**'ın mevcut olup olmadığını gösterir. |
| [ErrorString](../../aspose.cells.pivot/pivottable/errorstring/) { get; set; } | DisplayErrorString özelliği true olduğunda hatalar içeren hücrelerde gösterilen dizeyi alır. Varsayılan değer boş bir dizedir. |
| [ExternalConnectionDataSource](../../aspose.cells.pivot/pivottable/externalconnectiondatasource/) { get; } | (**Obsolete.**) Harici bağlantı veri kaynağını alır. |
| [FieldListSortAscending](../../aspose.cells.pivot/pivottable/fieldlistsortascending/) { get; set; } | **PivotTable** içindeki alanların alan listesinde varsayılan olmayan sırayla sıralanıp sıralanmadığını gösterir. |
| [FilterArea](../../aspose.cells.pivot/pivottable/filterarea/) { get; } | Filtre bölgesinin alanını alır. |
| [GrandTotalName](../../aspose.cells.pivot/pivottable/grandtotalname/) { get; set; } | Grand total sütun veya satır başlığında gösterilen etiketi döndürür. Varsayılan değer "Grand Total" dizesidir. |
| [HasBlankRows](../../aspose.cells.pivot/pivottable/hasblankrows/) { get; set; } | (**Obsolete.**) Boş satır eklenip eklenmeyeceğini gösterir. Bu özellik yalnızca boş satır eklenmesi gereken PivotTable otomatik biçim türleri için geçerlidir. |
| [Indent](../../aspose.cells.pivot/pivottable/indent/) { get; set; } | Kompakt eksen için girinti artışını belirtir ve Rapor Düzeni'ni Kompakt Formata ayarlamak için kullanılabilir. |
| [IsAutoFormat](../../aspose.cells.pivot/pivottable/isautoformat/) { get; set; } | **PivotTable** raporunun otomatik olarak biçimlendirilip biçimlendirilmediğini gösterir. Excel 2003'teki pivottable seçeneğinde bulunan "autoformat table" onay kutusu |
| [IsExcel2003Compatible](../../aspose.cells.pivot/pivottable/isexcel2003compatible/) { get; set; } | PivotTable yenilenirken **PivotTable**'ın Excel2003 ile uyumlu olup olmadığını belirtir; true ise bir dize 255 karakterden az veya eşit olmalıdır, 255 karakterden uzun ise kesilir. false ise dize bu sınırlamaya tabi değildir. Varsayılan değer true'tur. |
| [IsGridDropZones](../../aspose.cells.pivot/pivottable/isgriddropzones/) { get; set; } | **PivotTable** raporunun klasik pivottable düzenini gösterip göstermediğini belirtir. (ızgarada alanları sürüklemeyi etkinleştirir) |
| [IsMultipleFieldFilters](../../aspose.cells.pivot/pivottable/ismultiplefieldfilters/) { get; set; } | (**Obsolete.**) Bir **PivotTable**'ın alanlarının birden fazla filtreye sahip olup olamayacağını gösteren bir boolean değer belirtir. |
| [IsSelected](../../aspose.cells.pivot/pivottable/isselected/) { get; set; } | Bu **PivotTable**'ın seçili olup olmadığını gösterir. |
| [ItemPrintTitles](../../aspose.cells.pivot/pivottable/itemprinttitles/) { get; set; } | (**Obsolete.**) PivotItem adlarının her basılmış sayfanın üstünde tekrarlanıp tekrarlanmayacağını gösterir. |
| [ManualUpdate](../../aspose.cells.pivot/pivottable/manualupdate/) { get; set; } | **PivotTable** raporunun yalnızca kullanıcının talebi üzerine yeniden hesaplanıp hesaplanmayacağını gösterir. |
| [MergeLabels](../../aspose.cells.pivot/pivottable/mergelabels/) { get; set; } | Birden çok hücreye yayılan satır/sütun alan etiketlerinin birleştirilip birleştirilmeyeceğini alır veya ayarlar. |
| [MissingItemsLimit](../../aspose.cells.pivot/pivottable/missingitemslimit/) { get; set; } | (**Obsolete.**) Bir **PivotTable**'ın alanlarının birden fazla filtreye sahip olup olamayacağını gösteren bir boolean değer belirtir. |
| [Name](../../aspose.cells.pivot/pivottable/name/) { get; set; } | **PivotTable**'ın adını alır |
| [NullString](../../aspose.cells.pivot/pivottable/nullstring/) { get; set; } | DisplayNullString özelliği true olduğunda null değer içeren hücrelerde gösterilen dizeyi alır. Varsayılan değer boş bir dizedir. |
| [PageFieldOrder](../../aspose.cells.pivot/pivottable/pagefieldorder/) { get; set; } | Sayfa alanlarının **PivotTable** raporunun düzenine eklendiği sıralamayı alır ve ayarlar. |
| [PageFields](../../aspose.cells.pivot/pivottable/pagefields/) { get; } | Şu anda sayfa alanları olarak gösterilen bir [`PivotFieldCollection`](../pivotfieldcollection/) döndürür. |
| [PageFieldWrapCount](../../aspose.cells.pivot/pivottable/pagefieldwrapcount/) { get; set; } | **PivotTable** raporundaki her sütun veya satırdaki sayfa alanlarının sayısını alır. |
| [PivotCache](../../aspose.cells.pivot/pivottable/pivotcache/) { get; } | Veri kaynağını alır. |
| [PivotFilters](../../aspose.cells.pivot/pivottable/pivotfilters/) { get; } | Pivot tablo içindeki tüm filtreleri döndürür. |
| [PivotFormatConditions](../../aspose.cells.pivot/pivottable/pivotformatconditions/) { get; } | (**Obsolete.**) Pivot tablonun Biçim Koşullarını alır. |
| [PivotFormats](../../aspose.cells.pivot/pivottable/pivotformats/) { get; } | Bu pivot tabloya uygulanan tüm hücre biçimlerini alır. |
| [PivotTableStyle](../../aspose.cells.pivot/pivottable/pivottablestyle/) { get; set; } | Bu pivot tablonun TableStyle ayarlarını alır. |
| [PivotTableStyleName](../../aspose.cells.pivot/pivottable/pivottablestylename/) { get; set; } | Pivot tablonun stil adını alır veya ayarlar. |
| [PivotTableStyleType](../../aspose.cells.pivot/pivottable/pivottablestyletype/) { get; set; } | Yerleşik pivot tablo stilini alır ve ayarlar. |
| [PreserveCellFormattingOnUpdate](../../aspose.cells.pivot/pivottable/preservecellformattingonupdate/) { get; set; } | Pivot tablo yenilendiğinde veya yeniden hesaplandığında hücre biçimlendirmesinin ([`PivotTableFormat`](../pivottableformat/)) korunup korunmayacağını gösterir. |
| [PreserveFormatting](../../aspose.cells.pivot/pivottable/preserveformatting/) { get; set; } | (**Obsolete.**) PivotTable yenilendiğinde veya yeniden hesaplandığında hücre biçimlendirmesinin ([`PivotTableFormat`](../pivottableformat/)) korunup korunmadığını gösterir. |
| [PrintDrill](../../aspose.cells.pivot/pivottable/printdrill/) { get; set; } | Delme göstergelerinin yazdırılıp yazdırılmayacağını belirten bir boolean değer belirtir. Pivot tabloda görüntülendiğinde genişlet/küçült düğmelerini yazdır. |
| [PrintTitles](../../aspose.cells.pivot/pivottable/printtitles/) { get; set; } | Çalışma sayfası için yazdırma başlıklarının PivotTable raporuna göre ayarlanıp ayarlanmadığını gösterir. Varsayılan değer false'tur. |
| [RefreshDataOnOpeningFile](../../aspose.cells.pivot/pivottable/refreshdataonopeningfile/) { get; set; } | Dosya açıldığında Verileri Yenileme seçeneğinin etkin olup olmadığını gösterir. |
| [RefreshDate](../../aspose.cells.pivot/pivottable/refreshdate/) { get; } | PivotTable yenilendiği son tarih ve zamanı alır. |
| [RefreshedByWho](../../aspose.cells.pivot/pivottable/refreshedbywho/) { get; } | Bu PivotTable'ı yenileyen son kullanıcının adını alır. |
| [RepeatItemsOnEachPrintedPage](../../aspose.cells.pivot/pivottable/repeatitemsoneachprintedpage/) { get; set; } | Satır alanındaki pivot öğesi başlıklarının tablo biçimindeki pivot alanları için her yazdırılan sayfada tekrarlanıp tekrarlanmadığını gösterir. |
| [RowFields](../../aspose.cells.pivot/pivottable/rowfields/) { get; } | Şu anda satır alanı olarak gösterilen bir [`PivotFieldCollection`](../pivotfieldcollection/) döndürür. |
| [RowGrand](../../aspose.cells.pivot/pivottable/rowgrand/) { get; set; } | (**Obsolete.**) Bu pivot tablonun satırları için toplamları gösterip göstermeyeceğini gösterir. |
| [RowHeaderCaption](../../aspose.cells.pivot/pivottable/rowheadercaption/) { get; set; } | Bu PivotTable'daki Satır Başlığının özel başlığını alır ve ayarlar. |
| [RowRange](../../aspose.cells.pivot/pivottable/rowrange/) { get; } | PivotTable raporundaki satır alanını içeren aralığı temsil eden bir CellArea nesnesi döndürür. Salt okunur. |
| [SaveData](../../aspose.cells.pivot/pivottable/savedata/) { get; set; } | PivotTable raporu için verilerin çalışma kitabıyla birlikte kaydedilip kaydedilmediğini gösterir. |
| [ShowColumnGrandTotals](../../aspose.cells.pivot/pivottable/showcolumngrandtotals/) { get; set; } | Bu pivot tablonun sütunları için toplamları gösterip göstermeyeceğini gösterir. |
| [ShowDataTips](../../aspose.cells.pivot/pivottable/showdatatips/) { get; set; } | PivotTable veri hücreleri için araç ipuçlarının gösterilip gösterilmeyeceğini gösterir. |
| [ShowDrill](../../aspose.cells.pivot/pivottable/showdrill/) { get; set; } | Genişlet/küçült düğmelerinin gösterilip gösterilmeyeceğini alır ve ayarlar. |
| [ShowEmptyCol](../../aspose.cells.pivot/pivottable/showemptycol/) { get; set; } | Tabloda boş sütunların dahil edilip edilmeyeceğini gösterir. |
| [ShowEmptyRow](../../aspose.cells.pivot/pivottable/showemptyrow/) { get; set; } | Tabloda boş satırların dahil edilip edilmeyeceğini gösterir. |
| [ShowHeaders](../../aspose.cells.pivot/pivottable/showheaders/) { get; set; } | PivotTable görünümünde satır ekseninde ve sütun ekseninde veri alanı başlıklarını ve pivot alanı başlıklarını gösterip göstermeyeceği. |
| [ShowMemberPropertyTips](../../aspose.cells.pivot/pivottable/showmemberpropertytips/) { get; set; } | Üye özelliği bilgilerinin PivotTable araç ipuçlarından çıkarılıp çıkarılmayacağını belirten bir boolean değer belirtir. |
| [ShowPivotStyleColumnHeader](../../aspose.cells.pivot/pivottable/showpivotstylecolumnheader/) { get; set; } | Pivot tablo içindeki sütun başlığının stile uygulanıp uygulanmayacağını gösterir. |
| [ShowPivotStyleColumnStripes](../../aspose.cells.pivot/pivottable/showpivotstylecolumnstripes/) { get; set; } | Sütun için çizgili biçimlendirmenin uygulanıp uygulanmadığını gösterir. |
| [ShowPivotStyleLastColumn](../../aspose.cells.pivot/pivottable/showpivotstylelastcolumn/) { get; set; } | Sütun biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [ShowPivotStyleRowHeader](../../aspose.cells.pivot/pivottable/showpivotstylerowheader/) { get; set; } | Pivot tablo içindeki satır başlığının stile uygulanıp uygulanmayacağını gösterir. |
| [ShowPivotStyleRowStripes](../../aspose.cells.pivot/pivottable/showpivotstylerowstripes/) { get; set; } | Satır çizgili biçimlendirmenin uygulanıp uygulanmadığını gösterir. |
| [ShowRowGrandTotals](../../aspose.cells.pivot/pivottable/showrowgrandtotals/) { get; set; } | Pivot tablonun satırları için toplamların gösterilip gösterilmeyeceğini gösterir. |
| [ShowRowHeaderCaption](../../aspose.cells.pivot/pivottable/showrowheadercaption/) { get; set; } | (**Obsolete.**) Satır başlığı başlığının PivotTable raporunda gösterilip gösterilmediğini ve Alan başlıklarının ve filtre açılır menülerinin görüntülenip görüntülenmediğini gösterir. |
| [ShowValuesRow](../../aspose.cells.pivot/pivottable/showvaluesrow/) { get; set; } | Değerler satırının gösterilip gösterilmediğini gösterir. |
| [SourceType](../../aspose.cells.pivot/pivottable/sourcetype/) { get; } | Pivot tablonun veri kaynağı türünü alır. |
| [SubtotalHiddenPageItems](../../aspose.cells.pivot/pivottable/subtotalhiddenpageitems/) { get; set; } | PivotTable raporundaki gizli sayfa alanı öğelerinin satır ve sütun alt toplamlarına, blok toplamlarına ve genel toplamlarına dahil edilip edilmediğini gösterir. Varsayılan değer False'tur. |
| [TableRange1](../../aspose.cells.pivot/pivottable/tablerange1/) { get; } | Tüm PivotTable raporunu içeren ancak sayfa alanlarını içermeyen aralığı temsil eden bir CellArea nesnesi döndürür. Salt okunur. |
| [TableRange2](../../aspose.cells.pivot/pivottable/tablerange2/) { get; } | Tüm PivotTable raporunu ve sayfa alanlarını içeren aralığı temsil eden bir CellArea nesnesi döndürür. Salt okunur. |
| [Tag](../../aspose.cells.pivot/pivottable/tag/) { get; set; } | Bu PivotTable görünümüyle ilişkili kullanıcı tanımlı bir dizeyi alır ve ayarlar. |
| [TopRightArea](../../aspose.cells.pivot/pivottable/toprightarea/) { get; } | PivotTable'ın sağ üst (RTL sayfalar için sol üst) köşesindeki boş alanı temsil eder. |
| [ValuesField](../../aspose.cells.pivot/pivottable/valuesfield/) { get; } | Bir PivotTable'daki tüm veri alanlarını temsil eden bir [`PivotField`](../pivotfield/) nesnesini alır. Salt okunur. Veri bölgesinde iki veya daha fazla veri alanı olduğunda oluşturulur. Varsayılan olarak satır bölgesindedir. PivotTable.AddFieldToArea() yöntemiyle satır/sütun bölgesine sürükleyebilirsiniz. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield/#addcalculatedfield)(string, string) | Pivot alanına hesaplanmış bir alan ekler ve veri alanına sürükler. |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield/#addcalculatedfield_1)(string, string, bool) | Pivot alanına hesaplanmış bir alan ekler. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea_1)(PivotFieldType, int) | Alanı belirli alana ekler. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea)(PivotFieldType, PivotField) | Alanı belirli alana ekler. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea/#addfieldtoarea_2)(PivotFieldType, string) | Alanı belirli alana ekler. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata/#calculatedata_1)() | PivotTable verilerini hücrelere hesaplar. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata/#calculatedata)(PivotTableCalculateOption) | Seçeneklerle pivot tabloyu hesaplar. |
| [CalculateRange](../../aspose.cells.pivot/pivottable/calculaterange/)() | PivotTable'ın aralığını hesaplar. |
| [ChangeDataSource](../../aspose.cells.pivot/pivottable/changedatasource/)(string[]) | Pivot tablonun veri kaynağını değiştir. |
| [ClearAll](../../aspose.cells.pivot/pivottable/clearall/)() | Bölgelerden tüm alanları kaldır. |
| [ClearData](../../aspose.cells.pivot/pivottable/cleardata/)() | PivotTable görünümünün veri ve biçimlendirmesini temizle. |
| [ClearFilters](../../aspose.cells.pivot/pivottable/clearfilters/)() | Bu pivot tablonun tüm filtrelerini temizler. |
| [CopyStyle](../../aspose.cells.pivot/pivottable/copystyle/)(PivotTable) | Başka bir pivot tablodan adlandırılmış stili kopyalar. |
| [Dispose](../../aspose.cells.pivot/pivottable/dispose/)() | Yönetilmeyen kaynakların serbest bırakılması, salınması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür. |
| [ExportViewToJson](../../aspose.cells.pivot/pivottable/exportviewtojson/)(PivotViewToJsonOptions) | Pivot görünümünü JSON olarak dışa aktarır. |
| [Fields](../../aspose.cells.pivot/pivottable/fields/)(PivotFieldType) | (**Obsolete.**) Belirli alanları alan tipine göre alır. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format)(CellArea, Style) | PivotTable'ın seçili alanını biçimlendirir. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format_1)(PivotArea, Style) | PivotTable'ın seçili alanını biçimlendirir. |
| [Format](../../aspose.cells.pivot/pivottable/format/#format_2)(int, int, Style) | PivotTable alanındaki hücreyi biçimlendirir |
| [FormatAll](../../aspose.cells.pivot/pivottable/formatall/)(Style) | PivotTable alanındaki tüm hücreleri biçimlendir |
| [FormatRow](../../aspose.cells.pivot/pivottable/formatrow/)(int, Style) | PivotTable alanındaki satır verilerini biçimlendir |
| [GetButtonArea](../../aspose.cells.pivot/pivottable/getbuttonarea/)(PivotFieldType) | Alan düğmesini içeren bölgeyi alır. |
| [GetCellByDisplayName](../../aspose.cells.pivot/pivottable/getcellbydisplayname/)(string) | PivotField'ın görüntüleme adına göre [`Cell`](../../aspose.cells/cell/) nesnesini alır. |
| [GetChildren](../../aspose.cells.pivot/pivottable/getchildren/)() | (**Obsolete.**) Bu PivotTable verisini veri kaynağı olarak kullanan Children Pivot Tables'ı alır. |
| [GetDependentPivotTables](../../aspose.cells.pivot/pivottable/getdependentpivottables/)() | Bu PivotTable'ı veri kaynağı olarak kullanan tüm `PivotTable`'ları alır. |
| [GetFields](../../aspose.cells.pivot/pivottable/getfields/)(PivotFieldType) | Bölgeye göre belirli pivot alan listesini alır. |
| [GetHorizontalBreaks](../../aspose.cells.pivot/pivottable/gethorizontalbreaks/)() | (**Obsolete.**) Yatay sayfa sonlarının pivot tablo satır indeks listesini alır |
| [GetHorizontalPageBreaks](../../aspose.cells.pivot/pivottable/gethorizontalpagebreaks/)() | Bu pivot tablonun yatay sayfa sonlarını alır. |
| [GetNamesOfSourceDataConnections](../../aspose.cells.pivot/pivottable/getnamesofsourcedataconnections/)() | Harici kaynak veri bağlantılarının adlarını alır. |
| [GetPivotTablesWithSamePivotCache](../../aspose.cells.pivot/pivottable/getpivottableswithsamepivotcache/)() | Aynı pivot önbelleğine sahip tüm pivot tabloları alır. |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource/#getsource)() | Bu pivot tablonun veri kaynağını al. |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource/#getsource_1)(bool) | Bu pivot tablonun veri kaynağını al. |
| [GetSourceDataConnections](../../aspose.cells.pivot/pivottable/getsourcedataconnections/)() | Harici bağlantı veri kaynaklarını alır. |
| [Move](../../aspose.cells.pivot/pivottable/move/#move_1)(string) | (**Obsolete.**) PivotTable'ı çalışma sayfasında farklı bir konuma taşır. |
| [Move](../../aspose.cells.pivot/pivottable/move/#move)(int, int) | (**Obsolete.**) PivotTable'ı çalışma sayfasında farklı bir konuma taşır. |
| [MoveItem](../../aspose.cells.pivot/pivottable/moveitem/)(PivotFieldType, string[], bool, int) | Bir öğeyi yukarı ya da aşağı taşı. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto_2)(string) | PivotTable'ı çalışma sayfasında farklı bir konuma taşır. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto)(int, int) | PivotTable'ı çalışma sayfasında farklı bir konuma taşır. |
| [MoveTo](../../aspose.cells.pivot/pivottable/moveto/#moveto_1)(int, int, int) | PivotTable'ı çalışma sayfasında farklı bir konuma taşır. |
| [Refresh](../../aspose.cells.pivot/pivottable/refresh/#refresh)() | Veri kaynağından [`PivotCache`](./pivotcache/) yeniler ve pivot görünümü için veri ve stili hesaplar. |
| [Refresh](../../aspose.cells.pivot/pivottable/refresh/#refresh_1)(PivotTableRefreshOption) | Veri kaynağından [`PivotCache`](./pivotcache/) yeniler ve pivot görünümü için veri ve stili hesaplar. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata/#refreshdata)() | (**Obsolete.**) Veri kaynağından pivot önbelleğine verileri yeniler. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata/#refreshdata_1)(PivotTableRefreshOption) | (**Obsolete.**) PivotTable'ın verilerini ve ayarlarını veri kaynağından seçeneklerle yeniler. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield_1)(PivotFieldType, int) | Belirli pivot bölgeden bir alanı kaldırır. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield)(PivotFieldType, PivotField) | Belirli alan bölgesinden alanı kaldır |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield/#removefield_2)(PivotFieldType, string) | Belirli alan bölgesinden bir alanı kaldırır |
| [SelectArea](../../aspose.cells.pivot/pivottable/selectarea/)(CellArea) | Pivot tablo görünümünün bir alanını seçin. |
| [ShowDetail](../../aspose.cells.pivot/pivottable/showdetail/)(int, int, bool, int, int) | Veri bölgesindeki bir öğenin ayrıntısını yeni bir tabloya göster. |
| [ShowInCompactForm](../../aspose.cells.pivot/pivottable/showincompactform/)() | PivotTable görünümünü kompakt biçimde düzenler. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivottable/showinoutlineform/)() | PivotTable'ı taslak biçimde düzenler. |
| [ShowInTabularForm](../../aspose.cells.pivot/pivottable/showintabularform/)() | PivotTable'ı tablo biçiminde düzenler. |
| [ShowReportFilterPage](../../aspose.cells.pivot/pivottable/showreportfilterpage/)(PivotField) | PivotField'e göre tüm rapor filtre sayfalarını göster, PivotField PageFields içinde bulunmalıdır. |
| [ShowReportFilterPageByIndex](../../aspose.cells.pivot/pivottable/showreportfilterpagebyindex/)(int) | PageFields içindeki konum indeksine göre tüm rapor filtre sayfalarını göster. |
| [ShowReportFilterPageByName](../../aspose.cells.pivot/pivottable/showreportfilterpagebyname/)(string) | PivotField'in adına göre tüm rapor filtre sayfalarını göster, PivotField PageFields içinde bulunmalıdır. |

### Örnekler

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;

namespace AsposeCellsExamples
{
    public class PivotClassPivotTableDemo
    {
        public static void Run()
        {
            Workbook book = new Workbook();
            Worksheet sheet = book.Worksheets[0];
            Cells cells = sheet.Cells;

            // Örnek veriyi ayarla
            cells["A1"].Value = "fruit";
            cells["A2"].Value = "grape";
            cells["A3"].Value = "blueberry";
            cells["A4"].Value = "kiwi";
            cells["A5"].Value = "cherry";
            cells["A6"].Value = "grape";
            cells["A7"].Value = "blueberry";
            cells["A8"].Value = "kiwi";
            cells["A9"].Value = "cherry";

            cells["B1"].Value = "year";
            cells["B2"].Value = 2020;
            cells["B3"].Value = 2020;
            cells["B4"].Value = 2020;
            cells["B5"].Value = 2020;
            cells["B6"].Value = 2021;
            cells["B7"].Value = 2021;
            cells["B8"].Value = 2021;
            cells["B9"].Value = 2021;

            cells["C1"].Value = "amount";
            cells["C2"].Value = 50;
            cells["C3"].Value = 60;
            cells["C4"].Value = 70;
            cells["C5"].Value = 80;
            cells["C6"].Value = 90;
            cells["C7"].Value = 100;
            cells["C8"].Value = 110;
            cells["C9"].Value = 120;

            // Özet tablo oluştur
            PivotTableCollection pivots = sheet.PivotTables;
            int pivotIndex = pivots.Add("=Sheet1!A1:C9", "A12", "TestPivotTable");
            PivotTable pivot = pivots[pivotIndex];

            // Alanlar ekle
            pivot.AddFieldToArea(PivotFieldType.Row, "fruit");
            pivot.AddFieldToArea(PivotFieldType.Column, "year");
            pivot.AddFieldToArea(PivotFieldType.Data, "amount");

            // Pivot tabloyu biçimlendir
            pivot.PivotTableStyleType = PivotTableStyleType.PivotTableStyleMedium10;

            // Satır alanını özelleştir
            PivotField rowField = pivot.RowFields[0];
            rowField.DisplayName = "Fruit Category";

            // Verileri yenile ve hesapla
            pivot.RefreshData();
            pivot.CalculateData();

            // Çalışma kitabını kaydedin
            book.Save("PivotTableDemo.xlsx");
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)


