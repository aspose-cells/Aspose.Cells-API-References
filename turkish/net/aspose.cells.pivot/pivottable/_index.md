---
title: PivotTable
second_title: Aspose.Cells for .NET API Referansı
description: PivotTable. için özet açıklama
type: docs
weight: 4690
url: /tr/net/aspose.cells.pivot/pivottable/
---
## PivotTable class

PivotTable. için özet açıklama

```csharp
public class PivotTable : IDisposable
```

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AltTextDescription](../../aspose.cells.pivot/pivottable/alttextdescription) { get; set; } | Alt text öğesinin açıklamasını alır |
| [AltTextTitle](../../aspose.cells.pivot/pivottable/alttexttitle) { get; set; } | altertext başlığını alır |
| [AutoFormatType](../../aspose.cells.pivot/pivottable/autoformattype) { get; set; } | Özet Tablo otomatik biçim türünü alır. |
| [BaseFields](../../aspose.cells.pivot/pivottable/basefields) { get; } | Özet Tablo raporundaki tüm alanları içeren bir PivotFields nesnesi döndürür |
| [ColumnFields](../../aspose.cells.pivot/pivottable/columnfields) { get; } | Şu anda sütun alanları olarak gösterilen bir PivotFields nesnesi döndürür. |
| [ColumnGrand](../../aspose.cells.pivot/pivottable/columngrand) { get; set; } | Özet Tablo raporunun sütunlar için genel toplamları gösterip göstermediğini gösterir. |
| [ColumnHeaderCaption](../../aspose.cells.pivot/pivottable/columnheadercaption) { get; set; } | PivotTable'ın Sütun Başlığı Alt Yazısını Alır. |
| [ColumnRange](../../aspose.cells.pivot/pivottable/columnrange) { get; } | PivotTable raporundaki sütun alanını içeren aralığı temsil eden bir CellArea nesnesi döndürür. Salt okunur. |
| [CustomListSort](../../aspose.cells.pivot/pivottable/customlistsort) { get; set; } | data sıralanırken yerleşik özel listenin dikkate alınıp alınmayacağını belirtir |
| [DataBodyRange](../../aspose.cells.pivot/pivottable/databodyrange) { get; } | Üstbilgi satırı ile ekleme satırı arasındaki listede area verisini içeren aralığı temsil eden bir CellArea nesnesi döndürür. Salt okunur. |
| [DataField](../../aspose.cells.pivot/pivottable/datafield) { get; } | Bir PivotTable'daki tüm veri alanlarını temsil eden bir PivotField nesnesi alır. Salt okunur. Yalnızca DataPiovtFiels'te iki veya daha fazla veri alanı olduğunda başlatılır. Yalnızca DataPivotField'i PivotTable satırına/sütununa eklemek için kullanılır alan . Varsayılan satır alanındadır. |
| [DataFields](../../aspose.cells.pivot/pivottable/datafields) { get; } | Bir PivotTable'daki tüm veri alanlarını temsil eden bir PivotField nesnesi alır. Salt okunur. Yalnızca DataPiovtFiels'te iki veya daha fazla veri alanı olduğunda başlatılır. Yalnızca DataPivotField'i PivotTable satırına/sütununa eklemek için kullanılır alan . Varsayılan satır alanındadır. |
| [DataSource](../../aspose.cells.pivot/pivottable/datasource) { get; set; } | Pivot tablonun veri kaynağını alır ve ayarlar. |
| [DisplayErrorString](../../aspose.cells.pivot/pivottable/displayerrorstring) { get; set; } | PivotTable raporunun hata içeren hücrelerde özel bir dize gösterip göstermediğini gösterir. |
| [DisplayImmediateItems](../../aspose.cells.pivot/pivottable/displayimmediateitems) { get; set; } | PivotTable'ın veri alanı boş olduğunda satır ve sütun alanlarındaki öğelerin görünür olup olmadığını gösterir . Varsayılan değer true. |
| [DisplayNullString](../../aspose.cells.pivot/pivottable/displaynullstring) { get; set; } | PivotTable raporunun boş değerler içeren hücrelerde özel bir string gösterip göstermediğini gösterir. |
| [EnableDataValueEditing](../../aspose.cells.pivot/pivottable/enabledatavalueediting) { get; set; } | Kullanıcının pivot tablonun veri alanındaki hücreleri düzenlemesine izin verilip verilmediğini belirten bir boole değeri belirtir. field değerlerinde hücre düzenlemeyi etkinleştir |
| [EnableDrilldown](../../aspose.cells.pivot/pivottable/enabledrilldown) { get; set; } | Ayrıntılı incelemenin etkinleştirilip etkinleştirilmediğini alır. |
| [EnableFieldDialog](../../aspose.cells.pivot/pivottable/enablefielddialog) { get; set; } | Kullanıcı PivotTable alanını çift tıkladığında PivotTable Alanı iletişim kutusunun kullanılabilir olup olmadığını gösterir . |
| [EnableFieldList](../../aspose.cells.pivot/pivottable/enablefieldlist) { get; set; } | PivotTable için alan listesinin etkinleştirilip etkinleştirilmeyeceğini alır. |
| [EnableWizard](../../aspose.cells.pivot/pivottable/enablewizard) { get; set; } | Özet Tablo Sihirbazı'nın kullanılabilir olup olmadığını gösterir. |
| [ErrorString](../../aspose.cells.pivot/pivottable/errorstring) { get; set; } | DisplayErrorString özelliği true olduğunda error içeren hücrelerde görüntülenen dizeyi alır.Varsayılan değer boş bir dizedir. |
| [ExternalConnectionDataSource](../../aspose.cells.pivot/pivottable/externalconnectiondatasource) { get; } | Harici bağlantı veri kaynağını alır. |
| [FieldListSortAscending](../../aspose.cells.pivot/pivottable/fieldlistsortascending) { get; set; } | PivotTable'daki alanların alan listesinde varsayılan olmayan düzende sıralanıp sıralanmadığını gösteren bir boole değeri belirtir. |
| [GrandTotalName](../../aspose.cells.pivot/pivottable/grandtotalname) { get; set; } | Genel toplam sütununda veya satır başlığında görüntülenen metin dizesi etiketini döndürür. Varsayılan değer, "Genel Toplam" dizesidir. |
| [HasBlankRows](../../aspose.cells.pivot/pivottable/hasblankrows) { get; set; } | Boş satırların eklenip eklenmeyeceğini gösterir. Bu özellik yalnızca boş satırlar eklemesi gereken PivotTable otomatik format türleri için geçerlidir. |
| [Indent](../../aspose.cells.pivot/pivottable/indent) { get; set; } | Kompakt eksen için girinti artışını belirtir ve Rapor Düzenini Kompakt Form olarak ayarlamak için kullanılabilir. |
| [IsAutoFormat](../../aspose.cells.pivot/pivottable/isautoformat) { get; set; } | Özet Tablo raporunun otomatik olarak biçimlendirilip biçimlendirilmediğini gösterir. Excel 2003 için özetlenebilir seçenekte bulunan "tabloyu otomatik biçimlendir" onay kutusu Pivot tabloda bulunan "güncellemede sütun genişliğini otomatik sığdır" onay kutusu Seçenekler : Excel için Düzen Biçimi 2007 |
| [IsExcel2003Compatible](../../aspose.cells.pivot/pivottable/isexcel2003compatible) { get; set; } | Özet Tablo yenilenirken Özet Tablo'nun Excel2003 için uyumlu olup olmadığını belirtir, doğruysa, bir dize 255 karakterden küçük veya ona eşit olmalıdır, bu nedenle dize 255 karakterden büyükse, kesilecektir. false ise, bir dize yukarıda belirtilen kısıtlamaya sahip olmayacaktır. Varsayılan değer true'dur. |
| [IsGridDropZones](../../aspose.cells.pivot/pivottable/isgriddropzones) { get; set; } | PivotTable raporunun klasik pivot tablo düzenini gösterip göstermediğini gösterir. (ızgaradaki alanları sürüklemeyi etkinleştirir) |
| [IsMultipleFieldFilters](../../aspose.cells.pivot/pivottable/ismultiplefieldfilters) { get; set; } | Bir PivotTable alanlarının üzerlerinde ayarlanmış birden çok filtre olup olmayacağını belirten bir boole değeri belirtir. |
| [IsSelected](../../aspose.cells.pivot/pivottable/isselected) { get; set; } | PivotTable'ın seçili olup olmadığını gösterir. |
| [ItemPrintTitles](../../aspose.cells.pivot/pivottable/itemprinttitles) { get; set; } | axis satırındaki özet öğe başlıklarının, tablo biçimindeki pivot alanlar için yazdırılan her sayfada tekrarlanıp tekrarlanmayacağını belirten bir bit. |
| [ManualUpdate](../../aspose.cells.pivot/pivottable/manualupdate) { get; set; } | Özet Tablo raporunun yalnızca kullanıcının isteği üzerine yeniden hesaplanıp hesaplanmayacağını gösterir. |
| [MergeLabels](../../aspose.cells.pivot/pivottable/mergelabels) { get; set; } | Belirtilen PivotTable raporunun dış satır öğesi, sütun öğesi, ara toplam, ve genel toplam etiketlerinin birleştirilmiş hücreleri kullanıp kullanmadığını gösterir. |
| [MissingItemsLimit](../../aspose.cells.pivot/pivottable/missingitemslimit) { get; set; } | Bir PivotTable alanlarının üzerlerinde ayarlanmış birden çok filtre olup olmayacağını belirten bir boole değeri belirtir. |
| [Name](../../aspose.cells.pivot/pivottable/name) { get; set; } | PivotTable 'nin adını alır |
| [NullString](../../aspose.cells.pivot/pivottable/nullstring) { get; set; } | DisplayNullString özelliği true olduğunda boş değerler içeren hücrelerde görüntülenen dizeyi alır .Varsayılan değer boş bir dizedir. |
| [PageFieldOrder](../../aspose.cells.pivot/pivottable/pagefieldorder) { get; set; } | Sayfa alanlarının PivotTable raporunun düzenine eklenme sırasını alır. |
| [PageFields](../../aspose.cells.pivot/pivottable/pagefields) { get; } | Şu anda sayfa alanları olarak gösterilen bir PivotFields nesnesi döndürür. |
| [PageFieldWrapCount](../../aspose.cells.pivot/pivottable/pagefieldwrapcount) { get; set; } | PivotTable raporundaki her sütun veya satırdaki sayfa alanlarının sayısını alır. |
| [PivotFilters](../../aspose.cells.pivot/pivottable/pivotfilters) { get; } | Bir PivotFilterCollection nesnesi döndürür. |
| [PivotFormatConditions](../../aspose.cells.pivot/pivottable/pivotformatconditions) { get; } | Özet tablonun Biçim Koşullarını alır. |
| [PivotTableStyleName](../../aspose.cells.pivot/pivottable/pivottablestylename) { get; set; } | Özetlenebilir stil adını alır ve ayarlar. |
| [PivotTableStyleType](../../aspose.cells.pivot/pivottable/pivottablestyletype) { get; set; } | Yerleşik pivot tablo stilini alır ve ayarlar. |
| [PreserveFormatting](../../aspose.cells.pivot/pivottable/preserveformatting) { get; set; } | Özet Tablo yenilendiğinde veya yeniden hesaplandığında biçimlendirmenin korunup korunmadığını gösterir. |
| [PrintDrill](../../aspose.cells.pivot/pivottable/printdrill) { get; set; } | Delme göstergelerinin yazdırılıp yazdırılmayacağını belirten bir boole değeri belirtir. pivot tabloda görüntülendiğinde genişletme/daraltma düğmelerini yazdırın. |
| [PrintTitles](../../aspose.cells.pivot/pivottable/printtitles) { get; set; } | Çalışma sayfası için yazdırma başlıklarının PivotTable raporunda temelli ayarlanıp ayarlanmadığını gösterir. Varsayılan değer false. |
| [RefreshDataFlag](../../aspose.cells.pivot/pivottable/refreshdataflag) { get; set; } | Verileri Yenileyip Yenilemediğini gösterir. |
| [RefreshDataOnOpeningFile](../../aspose.cells.pivot/pivottable/refreshdataonopeningfile) { get; set; } | Dosyayı Açarken Verileri Yenileyip Yenilemediğini gösterir. |
| [RefreshDate](../../aspose.cells.pivot/pivottable/refreshdate) { get; } | PivotTable'ın en son yenilendiği tarihi alır. |
| [RefreshedByWho](../../aspose.cells.pivot/pivottable/refreshedbywho) { get; } | Özet Tabloyu en son yenileyen kullanıcının adını alır |
| [RowFields](../../aspose.cells.pivot/pivottable/rowfields) { get; } | Şu anda satır alanları olarak gösterilen bir PivotFields nesnesi döndürür. |
| [RowGrand](../../aspose.cells.pivot/pivottable/rowgrand) { get; set; } | Özet Tablo raporunun satırlar için genel toplamları gösterip göstermediğini gösterir. |
| [RowHeaderCaption](../../aspose.cells.pivot/pivottable/rowheadercaption) { get; set; } | PivotTable'ın Satır Başlığı Resim Yazısını Alır. |
| [RowRange](../../aspose.cells.pivot/pivottable/rowrange) { get; } | PivotTable raporundaki satır alanını içeren range aralığını temsil eden bir CellArea nesnesi döndürür. Salt okunur. |
| [SaveData](../../aspose.cells.pivot/pivottable/savedata) { get; set; } | PivotTable raporu verilerinin çalışma kitabıyla kaydedilip kaydedilmediğini gösterir. |
| [ShowDataTips](../../aspose.cells.pivot/pivottable/showdatatips) { get; set; } | PivotTable veri hücreleri için araç ipuçlarının görüntülenip görüntülenmeyeceğini belirten bir boole değeri belirtir. |
| [ShowDrill](../../aspose.cells.pivot/pivottable/showdrill) { get; set; } | Genişletme/daraltma düğmelerinin gösterilip gösterilmediğini alır. |
| [ShowEmptyCol](../../aspose.cells.pivot/pivottable/showemptycol) { get; set; } | Tabloya boş sütunların dahil edilip edilmeyeceğini gösteren bir boole değeri belirtir |
| [ShowEmptyRow](../../aspose.cells.pivot/pivottable/showemptyrow) { get; set; } | Tabloya boş satırların dahil edilip edilmeyeceğini gösteren bir boole değeri belirtir. |
| [ShowMemberPropertyTips](../../aspose.cells.pivot/pivottable/showmemberpropertytips) { get; set; } | Üye özellik bilgilerinin PivotTable araç ipuçlarından çıkarılması gerekip gerekmediğini belirten bir boole değeri belirtir. |
| [ShowPivotStyleColumnHeader](../../aspose.cells.pivot/pivottable/showpivotstylecolumnheader) { get; set; } | Pivot tablodaki sütun başlığına stilin uygulanıp uygulanmayacağını belirtir. |
| [ShowPivotStyleColumnStripes](../../aspose.cells.pivot/pivottable/showpivotstylecolumnstripes) { get; set; } | Sütun şerit biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [ShowPivotStyleLastColumn](../../aspose.cells.pivot/pivottable/showpivotstylelastcolumn) { get; set; } | Sütun şerit biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [ShowPivotStyleRowHeader](../../aspose.cells.pivot/pivottable/showpivotstylerowheader) { get; set; } | Pivot tablodaki satır başlığına stilin uygulanıp uygulanmayacağını belirtir. |
| [ShowPivotStyleRowStripes](../../aspose.cells.pivot/pivottable/showpivotstylerowstripes) { get; set; } | Satır şerit biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [ShowRowHeaderCaption](../../aspose.cells.pivot/pivottable/showrowheadercaption) { get; set; } | Satır başlığı başlığının PivotTable raporunda gösterilip gösterilmediğini gösterir Alan başlıklarını ve filtre açılır menülerini görüntüleyip görüntülemediğini gösterir |
| [ShowValuesRow](../../aspose.cells.pivot/pivottable/showvaluesrow) { get; set; } | Satır değerlerinin gösterilip gösterilmeyeceğini belirten bir boole değeri belirtir. row değerlerini gösterir |
| [SubtotalHiddenPageItems](../../aspose.cells.pivot/pivottable/subtotalhiddenpageitems) { get; set; } | Özet Tablo raporundaki gizli sayfa alanı öğelerinin satır ve sütun alt toplamlarına, blok toplamlarına ve genel toplamlara dahil edilip edilmediğini gösterir. Varsayılan değer False'dır. |
| [TableRange1](../../aspose.cells.pivot/pivottable/tablerange1) { get; } | PivotTable raporunun tamamını içeren aralığı temsil eden bir CellArea nesnesi döndürür, , ancak sayfa alanlarını içermez. Salt okunur. |
| [TableRange2](../../aspose.cells.pivot/pivottable/tablerange2) { get; } | PivotTable raporunun tamamını içeren aralığı temsil eden bir CellArea nesnesi döndürür, sayfa alanlarını içerir. Salt okunur. |
| [Tag](../../aspose.cells.pivot/pivottable/tag) { get; set; } | PivotTable raporuyla kaydedilmiş bir dize alır. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield#addcalculatedfield)(string, string) | Özet alanına hesaplanmış bir alan ekler ve onu veri alanına sürükler. |
| [AddCalculatedField](../../aspose.cells.pivot/pivottable/addcalculatedfield#addcalculatedfield_1)(string, string, bool) | Özet alanına hesaplanmış bir alan ekler. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea_1)(PivotFieldType, int) | Alanı belirli alana ekler. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea)(PivotFieldType, PivotField) | Alanı belirli alana ekler. |
| [AddFieldToArea](../../aspose.cells.pivot/pivottable/addfieldtoarea#addfieldtoarea_2)(PivotFieldType, string) | Alanı belirli alana ekler. |
| [CalculateData](../../aspose.cells.pivot/pivottable/calculatedata)() | Özet tablonun verilerini hücrelere hesaplar. |
| [CalculateRange](../../aspose.cells.pivot/pivottable/calculaterange)() | Özet tablonun aralığını hesaplar. |
| [ChangeDataSource](../../aspose.cells.pivot/pivottable/changedatasource)(string[]) | Özet tablonun kaynak verilerini ayarlayın. Sayfa1!$A$1:$C$3 |
| [ClearData](../../aspose.cells.pivot/pivottable/cleardata)() | PivotTable'ın verilerini ve biçimlendirmesini temizle |
| [CopyStyle](../../aspose.cells.pivot/pivottable/copystyle)(PivotTable) | Başka bir pivot tablodan adlandırılmış stili kopyalar. |
| [Dispose](../../aspose.cells.pivot/pivottable/dispose)() | Yönetilmeyen kaynakları serbest bırakma, serbest bırakma veya sıfırlama ile ilişkili uygulama tanımlı görevleri gerçekleştirir. |
| [Fields](../../aspose.cells.pivot/pivottable/fields)(PivotFieldType) | Alan türüne göre belirli alanları alır. |
| [Format](../../aspose.cells.pivot/pivottable/format)(int, int, Style) | Hücreyi döndürülebilir alanda biçimlendirin |
| [FormatAll](../../aspose.cells.pivot/pivottable/formatall)(Style) | Döndürülebilir alandaki tüm hücreyi biçimlendirin |
| [FormatRow](../../aspose.cells.pivot/pivottable/formatrow)(int, Style) | Özetlenebilir alandaki satır verilerini biçimlendirin |
| [GetCellByDisplayName](../../aspose.cells.pivot/pivottable/getcellbydisplayname)(string) | Cell nesnesini PivotField 'nin DisplayName değerine göre alır |
| [GetChildren](../../aspose.cells.pivot/pivottable/getchildren)() | Bu Özet Tablo verilerini veri kaynağı olarak kullanan Alt Özet Tabloları alır. |
| [GetHorizontalBreaks](../../aspose.cells.pivot/pivottable/gethorizontalbreaks)() | yatay sayfa sonlarının özet tablo satır dizin listesini al |
| [GetSource](../../aspose.cells.pivot/pivottable/getsource)() | Özet tablonun kaynak verilerini alın. |
| [Move](../../aspose.cells.pivot/pivottable/move#move_1)(string) | PivotTable'ı çalışma sayfasında farklı bir konuma taşır. |
| [Move](../../aspose.cells.pivot/pivottable/move#move)(int, int) | PivotTable'ı çalışma sayfasında farklı bir konuma taşır. |
| [RefreshData](../../aspose.cells.pivot/pivottable/refreshdata)() | Özet tablonun verilerini ve veri kaynağından gelen ayarları yeniler. |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield_1)(PivotFieldType, int) | Belirli bir alandan bir alanı kaldırır area |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield)(PivotFieldType, PivotField) | Alanı belirli alandan kaldır area |
| [RemoveField](../../aspose.cells.pivot/pivottable/removefield#removefield_2)(PivotFieldType, string) | Belirli bir alandan bir alanı kaldırır area |
| [SetAutoGroupField](../../aspose.cells.pivot/pivottable/setautogroupfield#setautogroupfield_1)(int) | Otomatik alan grubunu PivotTable'a göre ayarlar. |
| [SetAutoGroupField](../../aspose.cells.pivot/pivottable/setautogroupfield#setautogroupfield)(PivotField) | Otomatik alan grubunu PivotTable'a göre ayarlar. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_3)(int, DateTime, DateTime, ArrayList, int) | PivotTable'a göre manuel alan grubunu ayarlar. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_2)(int, double, double, ArrayList, double) | PivotTable'a göre manuel alan grubunu ayarlar. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield_1)(PivotField, DateTime, DateTime, ArrayList, int) | PivotTable'a göre manuel alan grubunu ayarlar. |
| [SetManualGroupField](../../aspose.cells.pivot/pivottable/setmanualgroupfield#setmanualgroupfield)(PivotField, double, double, ArrayList, double) | PivotTable'a göre manuel alan grubunu ayarlar. |
| [SetUngroup](../../aspose.cells.pivot/pivottable/setungroup#setungroup_1)(int) | Grubu PivotTable ile çözmeyi ayarlar |
| [SetUngroup](../../aspose.cells.pivot/pivottable/setungroup#setungroup)(PivotField) | Grubu PivotTable ile çözmeyi ayarlar |
| [ShowInCompactForm](../../aspose.cells.pivot/pivottable/showincompactform)() | PivotTable'ı kompakt biçimde düzenler. |
| [ShowInOutlineForm](../../aspose.cells.pivot/pivottable/showinoutlineform)() | PivotTable'ı anahat biçiminde düzenler. |
| [ShowInTabularForm](../../aspose.cells.pivot/pivottable/showintabularform)() | PivotTable'ı tablo biçiminde düzenler. |
| [ShowReportFilterPage](../../aspose.cells.pivot/pivottable/showreportfilterpage)(PivotField) | Tüm rapor filtresi sayfalarını PivotField'e göre göster, PivotField, PageFields'de bulunmalıdır. |
| [ShowReportFilterPageByIndex](../../aspose.cells.pivot/pivottable/showreportfilterpagebyindex)(int) | PageFields içindeki konum dizinine göre tüm rapor filtresi sayfalarını göster |
| [ShowReportFilterPageByName](../../aspose.cells.pivot/pivottable/showreportfilterpagebyname)(string) | Tüm rapor filtre sayfalarını PivotField adına göre göster, PivotField, PageFields. içinde bulunmalıdır. |

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

//PivotField'in özniteliklerini değiştir
PivotField rowField = pivot.RowFields[0];
rowField.DisplayName = "custom display name";

//PivotFilter'ı ekle
int index = pivot.PivotFilters.Add(0, PivotFilterType.Count);
PivotFilter filter = pivot.PivotFilters[index];
filter.AutoFilter.FilterTop10(0, false, false, 2);

//PivotFormatCondition Ekle
int formatIndex = pivot.PivotFormatConditions.Add();
PivotFormatCondition pfc = pivot.PivotFormatConditions[formatIndex];
FormatConditionCollection fcc = pfc.FormatConditions;
fcc.AddArea(pivot.DataBodyRange);
int idx = fcc.AddCondition(FormatConditionType.CellValue);
FormatCondition fc = fcc[idx];
fc.Formula1 = "100";
fc.Operator = OperatorType.GreaterOrEqual;
fc.Style.BackgroundColor = Color.Red;

pivot.RefreshData();
pivot.CalculateData();

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

'Change PivotField's attributes
Dim rowField As PivotField = pivot.RowFields(0)
rowField.DisplayName = "custom display name"

'PivotFilter Ekle
Dim filterIndex As Int32 = pivot.PivotFilters.Add(0, PivotFilterType.Count)
Dim filter As PivotFilter = pivot.PivotFilters(filterIndex)
filter.AutoFilter.FilterTop10(0, False, False, 2)

'PivotFormatCondition Ekle
Dim formatIndex As Int32 = pivot.PivotFormatConditions.Add()
Dim pfc As PivotFormatCondition = pivot.PivotFormatConditions(formatIndex)
Dim fcc As FormatConditionCollection = pfc.FormatConditions
fcc.AddArea(pivot.DataBodyRange)
Dim idx As Int32 = fcc.AddCondition(FormatConditionType.CellValue)
Dim fc As FormatCondition = fcc(idx)
fc.Formula1 = "100"
fc.Operator = OperatorType.GreaterOrEqual
fc.Style.BackgroundColor = Color.Red

pivot.RefreshData()
pivot.CalculateData()

book.Save("out_vb.xlsx")
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells.Pivot](../../aspose.cells.pivot)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
