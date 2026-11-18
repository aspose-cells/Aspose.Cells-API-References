---
title: "PivotTable Sınıfı"
linktitle: "PivotTable"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "PivotTable sınıfı. Go'da pivottable'ı temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/pivottable/
---

## PivotTable class

PivotTable için özet açıklama.

```go

type PivotTable struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [Dispose](./dispose/) | Yönetilmeyen kaynakları serbest bırakma, bırakma veya sıfırlama ile ilgili uygulama tanımlı görevleri yürütür. |
| [GetPivotCache](./getpivotcache/) | Veri kaynağını alır. |
| [IsExcel2003Compatible](./isexcel2003compatible/) | PivotTable yenilenirken PivotTable'ın Excel2003 ile uyumlu olup olmadığını belirtir, eğer true ise, bir dize 255 karakterden az veya eşit olmalıdır, bu yüzden dize 255 karakterden uzun olursa kırpılır. false ise, bir dize yukarıda belirtilen kısıtlamaya sahip olmayacaktır. Varsayılan değer true'tur. |
| [SetIsExcel2003Compatible](./setisexcel2003compatible/) | PivotTable yenilenirken PivotTable'ın Excel2003 ile uyumlu olup olmadığını belirtir, eğer true ise, bir dize 255 karakterden az veya eşit olmalıdır, bu yüzden dize 255 karakterden uzun olursa kırpılır. false ise, bir dize yukarıda belirtilen kısıtlamaya sahip olmayacaktır. Varsayılan değer true'tur. |
| [GetRefreshedByWho](./getrefreshedbywho/) | Bu PivotTable'ı yenileyen son kullanıcının adını alır. |
| [GetRefreshDate](./getrefreshdate/) | PivotTable yenilendiğinde son tarih ve saat bilgisini alır. |
| [GetPivotTableStyle](./getpivottablestyle/) | Bu pivot tablonun TableStyle ayarlarını alır. |
| [SetPivotTableStyle](./setpivottablestyle/) | Bu pivot tablonun TableStyle ayarlarını alır. |
| [GetPivotTableStyleName](./getpivottablestylename/) | Pivot tablonun stil adını alır veya ayarlar. |
| [SetPivotTableStyleName](./setpivottablestylename/) | Pivot tablonun stil adını alır veya ayarlar. |
| [GetPivotTableStyleType](./getpivottablestyletype/) | Yerleşik pivot tablo stilini alır ve ayarlar. |
| [SetPivotTableStyleType](./setpivottablestyletype/) | Yerleşik pivot tablo stilini alır ve ayarlar. |
| [CopyStyle](./copystyle/) | Başka bir pivot tablodan adlandırılmış stili kopyalar. |
| [ShowReportFilterPage](./showreportfilterpage/) | PivotField'a göre tüm rapor filtre sayfalarını göster, PivotField PageFields içinde bulunmalıdır. |
| [ShowReportFilterPageByName](./showreportfilterpagebyname/) | PivotField'ın adına göre tüm rapor filtre sayfalarını göster, PivotField PageFields içinde bulunmalıdır. |
| [ShowReportFilterPageByIndex](./showreportfilterpagebyindex/) | PageFields içindeki konum indeksine göre tüm rapor filtre sayfalarını göster. |
| [RemoveField_PivotFieldType_String](./removefield_pivotfieldtype_string/) | Belirli alan bölgesinden bir alanı kaldırır. |
| [RemoveField_PivotFieldType_Int](./removefield_pivotfieldtype_int/) | Belirli pivot bölgesinden bir alanı kaldırır. |
| [RemoveField_PivotFieldType_PivotField](./removefield_pivotfieldtype_pivotfield/) | Belirli alan bölgesinden alanı kaldır. |
| [AddFieldToArea_PivotFieldType_String](./addfieldtoarea_pivotfieldtype_string/) | Alanı belirli bölgeye ekler. |
| [AddFieldToArea_PivotFieldType_Int](./addfieldtoarea_pivotfieldtype_int/) | Alanı belirli bölgeye ekler. |
| [AddFieldToArea_PivotFieldType_PivotField](./addfieldtoarea_pivotfieldtype_pivotfield/) | Alanı belirli bölgeye ekler. |
| [AddCalculatedField_String_String_Bool](./addcalculatedfield_string_string_bool/) | Pivot alana hesaplanmış bir alan ekler. |
| [AddCalculatedField_String_String](./addcalculatedfield_string_string/) | Pivot alana hesaplanmış bir alan ekler ve veri bölgesine sürükler. |
| [GetFields](./getfields/) | Bölgeye göre belirli pivot alan listesini alır. |
| [GetColumnFields](./getcolumnfields/) | Şu anda sütun alanı olarak gösterilen bir PivotFields nesnesini döndürür. |
| [GetRowFields](./getrowfields/) | Şu anda satır alanı olarak gösterilen bir PivotFields nesnesini döndürür. |
| [GetPageFields](./getpagefields/) | Şu anda sayfa alanı olarak gösterilen bir PivotFields nesnesini döndürür. |
| [GetDataFields](./getdatafields/) | PivotTable'daki tüm veri alanlarını temsil eden bir PivotField nesnesini alır. Read-only. Yalnızca DataPivotFields içinde iki veya daha fazla veri alanı olduğunda başlatılır. Sadece DataPivotField'ı PivotTable satır/kolon bölgesine eklemek için kullanılır. Varsayılan olarak satır bölgesindedir. |
| [GetValuesField](./getvaluesfield/) | PivotTable'daki tüm veri alanlarını temsil eden bir PivotField nesnesini alır. Read-only. Yalnızca Veri bölgesinde iki veya daha fazla veri alanı olduğunda oluşturulur. Varsayılan olarak satır bölgesindedir. PivotTable.AddFieldToArea() yöntemiyle satır/kolon bölgesine sürüklenebilir. |
| [GetBaseFields](./getbasefields/) | PivotTable'daki tüm temel pivot alanlarını döndürür. |
| [GetPivotFilters](./getpivotfilters/) | Pivot tablo içindeki pivot alanların tüm filtrelerini döndürür. |
| [GetButtonArea](./getbuttonarea/) | Alan düğmesini içeren bölgeyi alır. |
| [GetTopRightArea](./gettoprightarea/) | PivotTable'ın sağ üst köşesindeki (RTL sayfalar için sol üst) boş alanı temsil eder. |
| [GetFilterArea](./getfilterarea/) | Filtre bölgesinin alanını alır. |
| [GetColumnRange](./getcolumnrange/) | PivotTable raporundaki sütun alanını içeren aralığı temsil eden bir CellArea nesnesi döndürür. Salt okunur. |
| [GetRowRange](./getrowrange/) | PivotTable raporundaki satır alanını içeren aralığı temsil eden bir CellArea nesnesi döndürür. Salt okunur. |
| [GetDataBodyRange](./getdatabodyrange/) | Başlık satırı ile ekleme satırı arasındaki listede veri alanını içeren aralığı temsil eden bir CellArea nesnesi döndürür. Salt okunur. |
| [GetTableRange1](./gettablerange1/) | Tüm PivotTable raporunu içeren, ancak sayfa alanlarını içermeyen aralığı temsil eden bir CellArea nesnesi döndürür. Salt okunur. |
| [GetTableRange2](./gettablerange2/) | Tüm PivotTable raporunu ve sayfa alanlarını içeren aralığı temsil eden bir CellArea nesnesi döndürür. Salt okunur. |
| [MoveTo_Int_Int](./moveto_int_int/) | PivotTable'ı çalışma sayfasında farklı bir konuma taşır. |
| [MoveTo_Int_Int_Int](./moveto_int_int_int/) | PivotTable'ı çalışma sayfasında farklı bir konuma taşır. |
| [MoveTo_String](./moveto_string/) | PivotTable'ı çalışma sayfasında farklı bir konuma taşır. |
| [IsGridDropZones](./isgriddropzones/) | PivotTable raporunun klasik pivottable düzenini gösterip göstermediğini belirtir. (ızgarada alanları sürüklemeyi etkinleştirir) |
| [SetIsGridDropZones](./setisgriddropzones/) | PivotTable raporunun klasik pivottable düzenini gösterip göstermediğini belirtir. (ızgarada alanları sürüklemeyi etkinleştirir) |
| [GetShowColumnGrandTotals](./getshowcolumngrandtotals/) | Bu pivot tablonun sütunları için genel toplamların gösterilip gösterilmeyeceğini belirtir. |
| [SetShowColumnGrandTotals](./setshowcolumngrandtotals/) | Bu pivot tablonun sütunları için genel toplamların gösterilip gösterilmeyeceğini belirtir. |
| [GetShowRowGrandTotals](./getshowrowgrandtotals/) | Pivot tablonun satırları için genel toplamların gösterilip gösterilmeyeceğini belirtir. |
| [SetShowRowGrandTotals](./setshowrowgrandtotals/) | Pivot tablonun satırları için genel toplamların gösterilip gösterilmeyeceğini belirtir. |
| [GetDisplayNullString](./getdisplaynullstring/) | PivotTable raporunun değer null olduğunda özel bir dize gösterip göstermediğini belirtir. |
| [SetDisplayNullString](./setdisplaynullstring/) | PivotTable raporunun değer null olduğunda özel bir dize gösterip göstermediğini belirtir. |
| [GetNullString](./getnullstring/) | DisplayNullString özelliği true olduğunda null değer içeren hücrelerde gösterilen dizeyi alır. Varsayılan değer boş bir dizedir. |
| [SetNullString](./setnullstring/) | DisplayNullString özelliği true olduğunda null değer içeren hücrelerde gösterilen dizeyi alır. Varsayılan değer boş bir dizedir. |
| [GetDisplayErrorString](./getdisplayerrorstring/) | PivotTable raporunun hata içeren hücrelerde özel bir dize gösterip göstermediğini belirtir. |
| [SetDisplayErrorString](./setdisplayerrorstring/) | PivotTable raporunun hata içeren hücrelerde özel bir dize gösterip göstermediğini belirtir. |
| [GetDataFieldHeaderName](./getdatafieldheadername/) | PivotTable'daki değer alanı alan başlığının adını alır ve ayarlar. |
| [SetDataFieldHeaderName](./setdatafieldheadername/) | PivotTable'daki değer alanı alan başlığının adını alır ve ayarlar. |
| [GetErrorString](./geterrorstring/) | DisplayErrorString özelliği true olduğunda hata içeren hücrelerde gösterilen dizeyi alır. Varsayılan değer boş bir dizedir. |
| [SetErrorString](./seterrorstring/) | DisplayErrorString özelliği true olduğunda hata içeren hücrelerde gösterilen dizeyi alır. Varsayılan değer boş bir dizedir. |
| [IsAutoFormat](./isautoformat/) | PivotTable raporunun otomatik biçimlendirilip biçimlendirilmediğini belirtir. Excel 2003'teki pivottable seçeneğinde bulunan "autoformat table" onay kutusu. |
| [SetIsAutoFormat](./setisautoformat/) | PivotTable raporunun otomatik biçimlendirilip biçimlendirilmediğini belirtir. Excel 2003'teki pivottable seçeneğinde bulunan "autoformat table" onay kutusu. |
| [GetAutofitColumnWidthOnUpdate](./getautofitcolumnwidthonupdate/) | Güncelleme sırasında sütun genişliğinin otomatik olarak ayarlanıp ayarlanmayacağını belirtir. |
| [SetAutofitColumnWidthOnUpdate](./setautofitcolumnwidthonupdate/) | Güncelleme sırasında sütun genişliğinin otomatik olarak ayarlanıp ayarlanmayacağını belirtir. |
| [GetAutoFormatType](./getautoformattype/) | PivotTable'ın otomatik biçim türünü alır ve ayarlar. |
| [SetAutoFormatType](./setautoformattype/) | PivotTable'ın otomatik biçim türünü alır ve ayarlar. |
| [GetMergeLabels](./getmergelabels/) | Birden fazla hücreye yayılan satır veya sütun başlıklarının tek bir hücrede birleştirilip birleştirilmeyeceğini belirtir. |
| [SetMergeLabels](./setmergelabels/) | Birden fazla hücreye yayılan satır veya sütun başlıklarının tek bir hücrede birleştirilip birleştirilmeyeceğini belirtir. |
| [GetPreserveCellFormattingOnUpdate](./getpreservecellformattingonupdate/) | Pivot tablo yenilendiğinde veya yeniden hesaplandığında hücre biçimlendirmesinin (PivotTableFormat) korunup korunmayacağını belirtir. |
| [SetPreserveCellFormattingOnUpdate](./setpreservecellformattingonupdate/) | Pivot tablo yenilendiğinde veya yeniden hesaplandığında hücre biçimlendirmesinin (PivotTableFormat) korunup korunmayacağını belirtir. |
| [GetShowDrill](./getshowdrill/) | Genişlet/küçült düğmelerinin gösterilip gösterilmeyeceğini alır ve ayarlar. |
| [SetShowDrill](./setshowdrill/) | Genişlet/küçült düğmelerinin gösterilip gösterilmeyeceğini alır ve ayarlar. |
| [GetEnableDrilldown](./getenabledrilldown/) | Drilldown'ın etkinleştirilip etkinleştirilmediğini belirtir. |
| [SetEnableDrilldown](./setenabledrilldown/) | Drilldown'ın etkinleştirilip etkinleştirilmediğini belirtir. |
| [GetEnableFieldDialog](./getenablefielddialog/) | Kullanıcı PivotTable alanına çift tıkladığında PivotTable Alanı iletişim kutusunun mevcut olup olmadığını belirtir. |
| [SetEnableFieldDialog](./setenablefielddialog/) | Kullanıcı PivotTable alanına çift tıkladığında PivotTable Alanı iletişim kutusunun mevcut olup olmadığını belirtir. |
| [GetEnableFieldList](./getenablefieldlist/) | Excel görünümünde PivotTable için alan listesinin mevcut olup olmadığını belirtir. |
| [SetEnableFieldList](./setenablefieldlist/) | Excel görünümünde PivotTable için alan listesinin mevcut olup olmadığını belirtir. |
| [GetEnableWizard](./getenablewizard/) | PivotTable Sihirbazının mevcut olup olmadığını belirtir. |
| [SetEnableWizard](./setenablewizard/) | PivotTable Sihirbazının mevcut olup olmadığını belirtir. |
| [GetSubtotalHiddenPageItems](./getsubtotalhiddenpageitems/) | PivotTable raporundaki gizli sayfa alanı öğelerinin satır ve sütun ara toplamlarına, blok toplamlarına ve genel toplamlarına dahil edilip edilmediğini belirtir. Varsayılan değer Yanlıştır. |
| [SetSubtotalHiddenPageItems](./setsubtotalhiddenpageitems/) | PivotTable raporundaki gizli sayfa alanı öğelerinin satır ve sütun ara toplamlarına, blok toplamlarına ve genel toplamlarına dahil edilip edilmediğini belirtir. Varsayılan değer Yanlıştır. |
| [GetGrandTotalName](./getgrandtotalname/) | Büyük toplam sütunu veya satır başlığında görüntülenen etiketi döndürür. Varsayılan değer "Grand Total" dizesidir. |
| [SetGrandTotalName](./setgrandtotalname/) | Büyük toplam sütunu veya satır başlığında görüntülenen etiketi döndürür. Varsayılan değer "Grand Total" dizesidir. |
| [GetManualUpdate](./getmanualupdate/) | PivotTable raporunun yalnızca kullanıcının isteğiyle yeniden hesaplanıp hesaplanmadığını gösterir. |
| [SetManualUpdate](./setmanualupdate/) | PivotTable raporunun yalnızca kullanıcının isteğiyle yeniden hesaplanıp hesaplanmadığını gösterir. |
| [GetAllowMultipleFiltersPerField](./getallowmultiplefiltersperfield/) | PivotTable alanlarının birden fazla filtreye sahip olup olamayacağını belirten bir boolean değer belirtir. |
| [SetAllowMultipleFiltersPerField](./setallowmultiplefiltersperfield/) | PivotTable alanlarının birden fazla filtreye sahip olup olamayacağını belirten bir boolean değer belirtir. |
| [GetEnableDataValueEditing](./getenabledatavalueediting/) | Kullanıcının pivottable veri alanındaki hücreleri düzenlemesine izin verilip verilmeyeceğini gösteren bir boolean değer belirtir. Değerler alanında hücre düzenlemeyi etkinleştir. |
| [SetEnableDataValueEditing](./setenabledatavalueediting/) | Kullanıcının pivottable veri alanındaki hücreleri düzenlemesine izin verilip verilmeyeceğini gösteren bir boolean değer belirtir. Değerler alanında hücre düzenlemeyi etkinleştir. |
| [GetShowDataTips](./getshowdatatips/) | PivotTable veri hücreleri için araç ipuçlarının gösterilip gösterilmeyeceğini belirtir. |
| [SetShowDataTips](./setshowdatatips/) | PivotTable veri hücreleri için araç ipuçlarının gösterilip gösterilmeyeceğini belirtir. |
| [GetShowMemberPropertyTips](./getshowmemberpropertytips/) | Üye özelliği bilgilerinin PivotTable araç ipuçlarından çıkarılıp çıkarılmayacağını gösteren bir boolean değer belirtir. |
| [SetShowMemberPropertyTips](./setshowmemberpropertytips/) | Üye özelliği bilgilerinin PivotTable araç ipuçlarından çıkarılıp çıkarılmayacağını gösteren bir boolean değer belirtir. |
| [GetShowValuesRow](./getshowvaluesrow/) | Değer satırının gösterilip gösterilmeyeceğini belirtir. |
| [SetShowValuesRow](./setshowvaluesrow/) | Değer satırının gösterilip gösterilmeyeceğini belirtir. |
| [GetShowEmptyCol](./getshowemptycol/) | Tabloda boş sütunların dahil edilip edilmeyeceğini belirtir. |
| [SetShowEmptyCol](./setshowemptycol/) | Tabloda boş sütunların dahil edilip edilmeyeceğini belirtir. |
| [GetShowEmptyRow](./getshowemptyrow/) | Tabloda boş satırların dahil edilip edilmeyeceğini belirtir. |
| [SetShowEmptyRow](./setshowemptyrow/) | Tabloda boş satırların dahil edilip edilmeyeceğini belirtir. |
| [GetFieldListSortAscending](./getfieldlistsortascending/) | PivotTable'daki alanların alan listesinde varsayılan olmayan bir sırayla sıralanıp sıralanmadığını belirtir. |
| [SetFieldListSortAscending](./setfieldlistsortascending/) | PivotTable'daki alanların alan listesinde varsayılan olmayan bir sırayla sıralanıp sıralanmadığını belirtir. |
| [GetPrintDrill](./getprintdrill/) | Delik göstergelerinin yazdırılıp yazdırılmayacağını gösteren bir boolean değer belirtir. Pivottable üzerinde görüntülendiğinde genişlet/küçült düğmelerini yazdır. |
| [SetPrintDrill](./setprintdrill/) | Delik göstergelerinin yazdırılıp yazdırılmayacağını gösteren bir boolean değer belirtir. Pivottable üzerinde görüntülendiğinde genişlet/küçült düğmelerini yazdır. |
| [GetAltTextTitle](./getalttexttitle/) | Alternatif metnin başlığını alır ve ayarlar. |
| [SetAltTextTitle](./setalttexttitle/) | Alternatif metnin başlığını alır ve ayarlar. |
| [GetAltTextDescription](./getalttextdescription/) | Alternatif metnin açıklamasını alır. |
| [SetAltTextDescription](./setalttextdescription/) | Alternatif metnin açıklamasını alır. |
| [GetName](./getname/) | PivotTable'ın adını alır. |
| [SetName](./setname/) | PivotTable'ın adını alır. |
| [GetColumnHeaderCaption](./getcolumnheadercaption/) | PivotTable'ın sütun başlığının özel başlığını alır ve ayarlar. |
| [SetColumnHeaderCaption](./setcolumnheadercaption/) | PivotTable'ın sütun başlığının özel başlığını alır ve ayarlar. |
| [GetIndent](./getindent/) | Kompakt eksen için girinti artışını belirtir ve Rapor Düzenini Kompakt Formata ayarlamak için kullanılabilir. |
| [SetIndent](./setindent/) | Kompakt eksen için girinti artışını belirtir ve Rapor Düzenini Kompakt Formata ayarlamak için kullanılabilir. |
| [GetRowHeaderCaption](./getrowheadercaption/) | Bu PivotTable'daki satır başlığının özel başlığını alır ve ayarlar. |
| [SetRowHeaderCaption](./setrowheadercaption/) | Bu PivotTable'daki satır başlığının özel başlığını alır ve ayarlar. |
| [GetShowHeaders](./getshowheaders/) | PivotTable görünümünde satır ekseninde ve sütun ekseninde veri alanı başlıklarının ve pivot alanı başlıklarının gösterilip gösterilmeyeceği. |
| [SetShowHeaders](./setshowheaders/) | PivotTable görünümünde satır ekseninde ve sütun ekseninde veri alanı başlıklarının ve pivot alanı başlıklarının gösterilip gösterilmeyeceği. |
| [GetCustomListSort](./getcustomlistsort/) | Veri sıralanırken yerleşik özel listenin dikkate alınıp alınmayacağını belirtir. |
| [SetCustomListSort](./setcustomlistsort/) | Veri sıralanırken yerleşik özel listenin dikkate alınıp alınmayacağını belirtir. |
| [GetConditionalFormats](./getconditionalformats/) | Pivot tabloyun koşullu biçimlendirmelerini alır. |
| [GetPageFieldOrder](./getpagefieldorder/) | Sayfa alanlarının PivotTable raporunun düzenine eklenme sırasını alır ve ayarlar. |
| [SetPageFieldOrder](./setpagefieldorder/) | Sayfa alanlarının PivotTable raporunun düzenine eklenme sırasını alır ve ayarlar. |
| [GetPageFieldWrapCount](./getpagefieldwrapcount/) | PivotTable raporundaki her sütun veya satırdaki sayfa alanı sayısını alır. |
| [SetPageFieldWrapCount](./setpagefieldwrapcount/) | PivotTable raporundaki her sütun veya satırdaki sayfa alanı sayısını alır. |
| [GetTag](./gettag/) | Bu PivotTable görünümüyle ilişkili kullanıcı tanımlı bir dizeyi alır ve ayarlar. |
| [SetTag](./settag/) | Bu PivotTable görünümüyle ilişkili kullanıcı tanımlı bir dizeyi alır ve ayarlar. |
| [GetSaveData](./getsavedata/) | PivotTable raporu verilerinin çalışma kitabıyla birlikte kaydedilip kaydedilmediğini belirtir. |
| [SetSaveData](./setsavedata/) | PivotTable raporu verilerinin çalışma kitabıyla birlikte kaydedilip kaydedilmediğini belirtir. |
| [GetRefreshDataOnOpeningFile](./getrefreshdataonopeningfile/) | Dosya açıldığında verilerin yenilenip yenilenmeyeceğini belirtir. |
| [SetRefreshDataOnOpeningFile](./setrefreshdataonopeningfile/) | Dosya açıldığında verilerin yenilenip yenilenmeyeceğini belirtir. |
| [GetSourceType](./getsourcetype/) | Pivot tablonun veri kaynağı türünü alır. |
| [GetSourceDataConnections](./getsourcedataconnections/) | Harici bağlantı veri kaynaklarını alır. |
| [GetNamesOfSourceDataConnections](./getnamesofsourcedataconnections/) | Harici kaynak veri bağlantılarının adlarını alır. |
| [GetDataSource](./getdatasource/) | Pivot tablonun veri kaynağını alır ve ayarlar. |
| [SetDataSource](./setdatasource/) | Pivot tablonun veri kaynağını alır ve ayarlar. |
| [ChangeDataSource](./changedatasource/) | Pivot tablonun veri kaynağını değiştir. |
| [GetSource](./getsource/) | Bu pivot tablonun veri kaynağını al. |
| [GetSource_Bool](./getsource_bool/) | Bu pivot tablonun veri kaynağını al. |
| [Refresh](./refresh/) | PivotCache'i veri kaynağından yenile ve pivot görünümü için veri ve stili hesapla. |
| [CalculateData](./calculatedata/) | Pivot tablonun verilerini hücrelere hesaplar. |
| [CalculateData_PivotTableCalculateOption](./calculatedata_pivottablecalculateoption/) | Seçeneklerle pivot tabloyu hesaplar. |
| [GetPivotTablesWithSamePivotCache](./getpivottableswithsamepivotcache/) | Aynı pivot önbelleğine sahip tüm pivot tabloları alır. |
| [ClearData](./cleardata/) | PivotTable görünümünün veri ve biçimlendirmesini temizle. |
| [ClearFilters](./clearfilters/) | Bu pivot tablonun tüm filtrelerini temizler. |
| [ClearAll](./clearall/) | Bölgelerden tüm alanları kaldır. |
| [CalculateRange](./calculaterange/) | Pivot tablonun aralığını hesaplar. |
| [FormatAll](./formatall/) | Pivot tablo alanındaki tüm hücreleri biçimlendir. |
| [FormatRow](./formatrow/) | Pivot tablo alanındaki satır verilerini biçimlendir. |
| [Format_PivotArea_Style](./format_pivotarea_style/) | PivotTable'ın seçili alanını biçimlendir. |
| [Format_CellArea_Style](./format_cellarea_style/) | PivotTable'ın seçili alanını biçimlendir. |
| [Format_Int_Int_Style](./format_int_int_style/) | Pivot tablo alanındaki hücreyi biçimlendir. |
| [SelectArea](./selectarea/) | Pivot tablo görünümünün bir alanını seç. |
| [ShowDetail](./showdetail/) | Veri bölgesindeki bir öğenin ayrıntısını yeni bir tabloya göster. |
| [GetPivotFormats](./getpivotformats/) | PivotTable'a uygulanan tüm biçimleri al. |
| [GetRepeatItemsOnEachPrintedPage](./getrepeatitemsoneachprintedpage/) | Satır alanındaki pivot öğesi başlıklarının tablo biçimindeki pivot alanları için her basılan sayfada tekrarlanıp tekrarlanmayacağını gösterir. |
| [SetRepeatItemsOnEachPrintedPage](./setrepeatitemsoneachprintedpage/) | Satır alanındaki pivot öğesi başlıklarının tablo biçimindeki pivot alanları için her basılan sayfada tekrarlanıp tekrarlanmayacağını gösterir. |
| [GetPrintTitles](./getprinttitles/) | Çalışma sayfası için yazdırma başlıklarının PivotTable raporuna göre ayarlanıp ayarlanmadığını gösterir. Varsayılan değer false'tur. |
| [SetPrintTitles](./setprinttitles/) | Çalışma sayfası için yazdırma başlıklarının PivotTable raporuna göre ayarlanıp ayarlanmadığını gösterir. Varsayılan değer false'tur. |
| [GetDisplayImmediateItems](./getdisplayimmediateitems/) | PivotTable'ın veri alanı boş olduğunda satır ve sütun alanlarındaki öğelerin görünür olup olmadığını gösterir. Varsayılan değer true'dur. |
| [SetDisplayImmediateItems](./setdisplayimmediateitems/) | PivotTable'ın veri alanı boş olduğunda satır ve sütun alanlarındaki öğelerin görünür olup olmadığını gösterir. Varsayılan değer true'dur. |
| [IsSelected](./isselected/) | Bu PivotTable'ın seçili olup olmadığını gösterir. |
| [SetIsSelected](./setisselected/) | Bu PivotTable'ın seçili olup olmadığını gösterir. |
| [GetShowPivotStyleRowHeader](./getshowpivotstylerowheader/) | Pivot tablo içindeki satır başlığının stile uygulanıp uygulanmayacağını gösterir. |
| [SetShowPivotStyleRowHeader](./setshowpivotstylerowheader/) | Pivot tablo içindeki satır başlığının stile uygulanıp uygulanmayacağını gösterir. |
| [GetShowPivotStyleColumnHeader](./getshowpivotstylecolumnheader/) | Pivot tablo içindeki sütun başlığının stile uygulanıp uygulanmayacağını gösterir. |
| [SetShowPivotStyleColumnHeader](./setshowpivotstylecolumnheader/) | Pivot tablo içindeki sütun başlığının stile uygulanıp uygulanmayacağını gösterir. |
| [GetShowPivotStyleRowStripes](./getshowpivotstylerowstripes/) | Satır şerit biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [SetShowPivotStyleRowStripes](./setshowpivotstylerowstripes/) | Satır şerit biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [GetShowPivotStyleColumnStripes](./getshowpivotstylecolumnstripes/) | Sütun için şerit biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [SetShowPivotStyleColumnStripes](./setshowpivotstylecolumnstripes/) | Sütun için şerit biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [GetShowPivotStyleLastColumn](./getshowpivotstylelastcolumn/) | Sütun biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [SetShowPivotStyleLastColumn](./setshowpivotstylelastcolumn/) | Sütun biçimlendirmesinin uygulanıp uygulanmadığını gösterir. |
| [GetHorizontalPageBreaks](./gethorizontalpagebreaks/) | Bu pivot tablonun yatay sayfa sonlarını alır. |
| [ShowInCompactForm](./showincompactform/) | PivotTable görünümünü kompakt biçimde düzenler. |
| [ShowInOutlineForm](./showinoutlineform/) | PivotTable'ı taslak biçimde düzenler. |
| [ShowInTabularForm](./showintabularform/) | PivotTable'ı tablo biçiminde düzenler. |
| [GetCellByDisplayName](./getcellbydisplayname/) | PivotField'in görüntüleme adıyla Cell nesnesini alır. |
| [GetDependentPivotTables](./getdependentpivottables/) | Bu PivotTable'ı veri kaynağı olarak kullanan tüm PivotTable'ları alır. |
| [ExportViewToJson](./exportviewtojson/) | Pivot görünümünü JSON olarak dışa aktarır. |
