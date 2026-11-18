---
title: "Worksheet Sınıfı"
linktitle: "Worksheet"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "Worksheet sınıfı. Go'da çalışma sayfasını temsil eden nesneyi kapsar."
type: docs
weight: 200
url: /tr/go-cpp/worksheet/
---

## Worksheet class

Tek bir çalışma sayfasını temsil eden nesneyi kapsüller.

```go

type Worksheet struct  {
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
| [GetProtection](./getprotection/) | Bir çalışma sayfası için mevcut olan çeşitli koruma seçeneklerini temsil eder. ExcelXP ve üzeri sürümlerde gelişmiş koruma seçeneklerini destekler. |
| [GetUniqueId](./getuniqueid/) | Benzersiz kimliği alır ve ayarlar, {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F} ile aynıdır. |
| [SetUniqueId](./setuniqueid/) | Benzersiz kimliği alır ve ayarlar, {15DB5C3C-A5A1-48AF-8F25-3D86AC232D4F} ile aynıdır. |
| [GetPanes](./getpanes/) | Pencere bölmelerini alır. |
| [GetWorkbook](./getworkbook/) | Bu sayfayı içeren çalışma kitabı nesnesini alır. |
| [GetCells](./getcells/) | Aspose.Cells.Cells koleksiyonunu alır. |
| [GetQueryTables](./getquerytables/) | Çalışma sayfasındaki QueryTableCollection'ı alır. |
| [GetType](./gettype/) | Çalışma sayfası türünü temsil eder. |
| [SetType](./settype/) | Çalışma sayfası türünü temsil eder. |
| [GetName](./getname/) | Çalışma sayfasının adını alır veya ayarlar. |
| [SetName](./setname/) | Çalışma sayfasının adını alır veya ayarlar. |
| [GetShowFormulas](./getshowformulas/) | Formüllerin mi yoksa sonuçlarının mı gösterileceğini belirtir. |
| [SetShowFormulas](./setshowformulas/) | Formüllerin mi yoksa sonuçlarının mı gösterileceğini belirtir. |
| [GetShowDataTypeIcons](./getshowdatatypeicons/) | Veri türü simgelerinin gösterilip gösterilmeyeceğini belirtir. |
| [SetShowDataTypeIcons](./setshowdatatypeicons/) | Veri türü simgelerinin gösterilip gösterilmeyeceğini belirtir. |
| [IsGridlinesVisible](./isgridlinesvisible/) | Kılavuz çizgilerinin görünür olup olmadığını gösteren bir değeri alır veya ayarlar. Varsayılan true'dur. |
| [SetIsGridlinesVisible](./setisgridlinesvisible/) | Kılavuz çizgilerinin görünür olup olmadığını gösteren bir değeri alır veya ayarlar. Varsayılan true'dur. |
| [IsRowColumnHeadersVisible](./isrowcolumnheadersvisible/) | Çalışma sayfasının satır ve sütun başlıklarını gösterip göstermeyeceğini belirten bir değeri alır veya ayarlar. Varsayılan true'dur. |
| [SetIsRowColumnHeadersVisible](./setisrowcolumnheadersvisible/) | Çalışma sayfasının satır ve sütun başlıklarını gösterip göstermeyeceğini belirten bir değeri alır veya ayarlar. Varsayılan true'dur. |
| [GetPaneState](./getpanestate/) | Bölmenin yatay veya dikey bölünmeleri olup olmadığını ve bu bölünmelerin dondurulup dondurulmadığını belirtir. |
| [GetDisplayZeros](./getdisplayzeros/) | Sıfır değerleri gösteriliyorsa true. |
| [SetDisplayZeros](./setdisplayzeros/) | Sıfır değerleri gösteriliyorsa true. |
| [GetDisplayRightToLeft](./getdisplayrighttoleft/) | Belirtilen çalışma sayfasının soldan sağa yerine sağdan sola gösterilip gösterilmediğini belirtir. Varsayılan false'tur. |
| [SetDisplayRightToLeft](./setdisplayrighttoleft/) | Belirtilen çalışma sayfasının soldan sağa yerine sağdan sola gösterilip gösterilmediğini belirtir. Varsayılan false'tur. |
| [IsOutlineShown](./isoutlineshown/) | Ana hatın gösterilip gösterilmeyeceğini belirtir. |
| [SetIsOutlineShown](./setisoutlineshown/) | Ana hatın gösterilip gösterilmeyeceğini belirtir. |
| [IsSelected](./isselected/) | Çalışma kitabı açıldığında bu çalışma sayfasının seçili olup olmadığını belirtir. |
| [SetIsSelected](./setisselected/) | Çalışma kitabı açıldığında bu çalışma sayfasının seçili olup olmadığını belirtir. |
| [FreezePanes_Int_Int_Int_Int](./freezepanes_int_int_int_int/) | Çalışma sayfasındaki belirtilen hücrede bölmeleri dondurur. |
| [GetFreezedPanes](./getfreezedpanes/) | Dondurulmuş bölmeleri alır. |
| [Split](./split/) | Pencereyi böler. |
| [FreezePanes_String_Int_Int](./freezepanes_string_int_int/) | Çalışma sayfasındaki belirtilen hücrede bölmeleri dondurur. |
| [UnFreezePanes](./unfreezepanes/) | Çalışma sayfasındaki bölmeleri dondurmayı kaldırır. |
| [RemoveSplit](./removesplit/) | Bölünmüş pencereyi kaldırır. |
| [GetPivotTables](./getpivottables/) | Bu çalışma sayfasındaki tüm pivot tabloları alır. |
| [GetListObjects](./getlistobjects/) | Bu çalışma sayfasındaki tüm ListObject'leri alır. |
| [GetTabId](./gettabid/) | Sayfa için dahili tanımlayıcıyı belirtir. |
| [SetTabId](./settabid/) | Sayfa için dahili tanımlayıcıyı belirtir. |
| [GetHorizontalPageBreaks](./gethorizontalpagebreaks/) | HorizontalPageBreakCollection koleksiyonunu alır. |
| [GetVerticalPageBreaks](./getverticalpagebreaks/) | VerticalPageBreakCollection koleksiyonunu alır. |
| [AddPageBreaks](./addpagebreaks/) | Sayfa sonu ekler. |
| [GetHyperlinks](./gethyperlinks/) | HyperlinkCollection koleksiyonunu alır. |
| [Copy_Worksheet](./copy_worksheet/) | Başka bir çalışma sayfasından içerikleri ve biçimleri kopyalar. |
| [Copy_Worksheet_CopyOptions](./copy_worksheet_copyoptions/) | Başka bir çalışma sayfasından içerikleri ve biçimleri kopyalar. |
| [AutoFitColumn_Int_Int_Int](./autofitcolumn_int_int_int/) | Sütun genişliğini otomatik olarak ayarlar. |
| [AutoFitColumns](./autofitcolumns/) | Bu çalışma sayfasındaki tüm sütunları otomatik olarak ayarlar. |
| [AutoFitColumns_AutoFitterOptions](./autofitcolumns_autofitteroptions/) | Bu çalışma sayfasındaki tüm sütunları otomatik olarak ayarlar. |
| [AutoFitColumn_Int](./autofitcolumn_int/) | Sütun genişliğini otomatik olarak ayarlar. |
| [AutoFitColumns_Int_Int](./autofitcolumns_int_int/) | Sütunların genişliğini otomatik olarak ayarlar. |
| [AutoFitColumns_Int_Int_AutoFitterOptions](./autofitcolumns_int_int_autofitteroptions/) | Sütunların genişliğini otomatik olarak ayarlar. |
| [AutoFitColumns_Int_Int_Int_Int](./autofitcolumns_int_int_int_int/) | Sütunların genişliğini otomatik olarak ayarlar. |
| [AutoFitColumns_Int_Int_Int_Int_AutoFitterOptions](./autofitcolumns_int_int_int_int_autofitteroptions/) | Sütunların genişliğini otomatik olarak ayarlar. |
| [AutoFitRow_Int_Int_Int](./autofitrow_int_int_int/) | Satır yüksekliğini otomatik olarak ayarlar. |
| [AutoFitRow_Int_Int_Int_AutoFitterOptions](./autofitrow_int_int_int_autofitteroptions/) | Satır yüksekliğini otomatik olarak ayarlar. |
| [AutoFitRows](./autofitrows/) | Bu çalışma sayfasındaki tüm satırları otomatik olarak ayarlar. |
| [AutoFitRows_Bool](./autofitrows_bool/) | Bu çalışma sayfasındaki tüm satırları otomatik olarak ayarlar. |
| [AutoFitRows_AutoFitterOptions](./autofitrows_autofitteroptions/) | Bu çalışma sayfasındaki tüm satırları otomatik olarak ayarlar. |
| [AutoFitRows_Int_Int](./autofitrows_int_int/) | Bir aralıktaki satır yüksekliğini otomatik olarak ayarlar. |
| [AutoFitRows_Int_Int_AutoFitterOptions](./autofitrows_int_int_autofitteroptions/) | Bir aralıktaki satır yüksekliğini otomatik olarak ayarlar. |
| [AutoFitRow_Int_Int_Int_Int](./autofitrow_int_int_int_int/) | Dikdörtgen bir aralıktaki satır yüksekliğini otomatik olarak ayarlar. |
| [AutoFitRow_Int](./autofitrow_int/) | Satır yüksekliğini otomatik olarak ayarlar. |
| [GetPageSetup](./getpagesetup/) | Bu sayfadaki sayfa ayarı açıklamasını temsil eder. |
| [GetAutoFilter](./getautofilter/) | Belirtilen çalışma sayfası için otomatik filtreyi temsil eder. |
| [Filter](./filter/) | Aralığı filtreler. |
| [GetAdvancedFilter](./getadvancedfilter/) | Gelişmiş filtrenin ayarlarını alır. |
| [Advanced_Filter](./advanced_filter/) | Verileri karmaşık ölçütlerle filtreler. |
| [RemoveAutoFilter](./removeautofilter/) | Çalışma sayfasının otomatik filtresini kaldırır. |
| [GetHasAutofilter](./gethasautofilter/) | Bu çalışma sayfasının otomatik filtreye sahip olup olmadığını gösterir. |
| [GetTransitionEvaluation](./gettransitionevaluation/) | Geçiş Formül Değerlendirmesi (Lotus uyumluluğu) seçeneğinin etkin olup olmadığını gösterir. |
| [SetTransitionEvaluation](./settransitionevaluation/) | Geçiş Formül Değerlendirmesi (Lotus uyumluluğu) seçeneğinin etkin olup olmadığını gösterir. |
| [GetTransitionEntry](./gettransitionentry/) | Geçiş Formül Girişi (Lotus uyumluluğu) seçeneğinin etkin olup olmadığını gösterir. |
| [SetTransitionEntry](./settransitionentry/) | Geçiş Formül Girişi (Lotus uyumluluğu) seçeneğinin etkin olup olmadığını gösterir. |
| [GetVisibilityType](./getvisibilitytype/) | Bu sayfanın görünür durumunu gösterir. |
| [SetVisibilityType](./setvisibilitytype/) | Bu sayfanın görünür durumunu gösterir. |
| [SetVisible](./setvisible/) | Görünür seçenekleri ayarlar. |
| [IsVisible](./isvisible/) | Çalışma sayfasının görünür olup olmadığını temsil eder. |
| [SetIsVisible](./setisvisible/) | Çalışma sayfasının görünür olup olmadığını temsil eder. |
| [SelectRange](./selectrange/) | Bir aralığı seçer. |
| [RemoveAllDrawingObjects](./removealldrawingobjects/) | Bu çalışma sayfasındaki tüm çizim nesnelerini kaldırır. |
| [ClearComments](./clearcomments/) | Tasarımcı elektronik tablosundaki tüm yorumları temizler. |
| [GetSparklineGroups](./getsparklinegroups/) | Çalışma sayfasındaki sparkline gruplarını alır. |
| [GetCharts](./getcharts/) | Bir Grafik koleksiyonunu alır |
| [GetComments](./getcomments/) | Yorum koleksiyonunu alır. |
| [GetPictures](./getpictures/) | Bir Resim koleksiyonunu alır. |
| [GetAllPictures](./getallpictures/) | Hücreye gömülü ve hücrelerin üzerindeki görüntüler dahil olmak üzere tüm resimleri alır. |
| [GetTextBoxes](./gettextboxes/) | Bir MetinKutusu koleksiyonunu alır. |
| [GetCheckBoxes](./getcheckboxes/) | Bir OnayKutusu koleksiyonunu alır. |
| [GetOleObjects](./getoleobjects/) | Bir çalışma sayfasındaki OleObject koleksiyonunu temsil eder. |
| [GetShapes](./getshapes/) | Bu çalışma sayfasındaki tüm çizim şekillerini döndürür. |
| [GetSlicers](./getslicers/) | Çalışma sayfasındaki Dilimleyici koleksiyonunu al |
| [GetTimelines](./gettimelines/) | Çalışma sayfasındaki Zaman Çizelgesi koleksiyonunu al |
| [Protect_ProtectionType](./protect_protectiontype/) | Çalışma sayfasını korur. |
| [Protect_ProtectionType_String_String](./protect_protectiontype_string_string/) | Çalışma sayfasını korur. |
| [Unprotect](./unprotect/) | Çalışma sayfasının korumasını kaldırır. |
| [Unprotect_String](./unprotect_string/) | Çalışma sayfasının korumasını kaldırır. |
| [GetIndex](./getindex/) | Çalışma sayfası koleksiyonundaki sayfanın dizinini alır. |
| [MoveTo](./moveto/) | Sayfayı elektronik tabloda başka bir konuma taşır. |
| [IsProtected](./isprotected/) | Çalışma sayfasının korumalı olup olmadığını gösterir. |
| [GetValidations](./getvalidations/) | Çalışma sayfasındaki veri doğrulama ayarları koleksiyonunu alır. |
| [GetAllowEditRanges](./getalloweditranges/) | Çalışma sayfasındaki düzenleme izni aralıkları koleksiyonunu alır. |
| [GetErrorCheckOptions](./geterrorcheckoptions/) | Belirli aralıklara uygulanan hata denetimi ayarını alır. |
| [GetOutline](./getoutline/) | Bu çalışma sayfasındaki ana hatları alır. |
| [GetFirstVisibleRow](./getfirstvisiblerow/) | İlk görünen satır dizinini temsil eder. |
| [SetFirstVisibleRow](./setfirstvisiblerow/) | İlk görünen satır dizinini temsil eder. |
| [GetFirstVisibleColumn](./getfirstvisiblecolumn/) | İlk görünen sütun dizinini temsil eder. |
| [SetFirstVisibleColumn](./setfirstvisiblecolumn/) | İlk görünen sütun dizinini temsil eder. |
| [Replace](./replace/) | Tüm hücrelerin metnini yeni bir dizeyle değiştirir. |
| [GetZoom](./getzoom/) | Yüzde olarak ölçek faktörünü temsil eder. 10 ile 400 arasında olmalıdır. |
| [SetZoom](./setzoom/) | Yüzde olarak ölçek faktörünü temsil eder. 10 ile 400 arasında olmalıdır. |
| [GetViewType](./getviewtype/) | Görünüm türünü alır ve ayarlar. |
| [SetViewType](./setviewtype/) | Görünüm türünü alır ve ayarlar. |
| [IsPageBreakPreview](./ispagebreakpreview/) | Belirtilen çalışma sayfasının normal görünümde mi yoksa sayfa sonu önizlemesinde mi gösterileceğini belirtir. |
| [SetIsPageBreakPreview](./setispagebreakpreview/) | Belirtilen çalışma sayfasının normal görünümde mi yoksa sayfa sonu önizlemesinde mi gösterileceğini belirtir. |
| [IsRulerVisible](./isrulervisible/) | Cetvelin görünür olup olmadığını belirtir. Bu özellik yalnızca sayfa sonu önizlemesinde uygulanır. |
| [SetIsRulerVisible](./setisrulervisible/) | Cetvelin görünür olup olmadığını belirtir. Bu özellik yalnızca sayfa sonu önizlemesinde uygulanır. |
| [GetSelectedAreas](./getselectedareas/) | Tasarımcı elektronik tabloda seçili hücre aralıklarını alır. |
| [GetTabColor](./gettabcolor/) | Çalışma sayfası sekmesi rengini temsil eder. |
| [SetTabColor](./settabcolor/) | Çalışma sayfası sekmesi rengini temsil eder. |
| [GetGridlineColor](./getgridlinecolor/) | Kılavuz çizgi rengini alır ve ayarlar. |
| [SetGridlineColor](./setgridlinecolor/) | Kılavuz çizgi rengini alır ve ayarlar. |
| [GetCodeName](./getcodename/) | Çalışma sayfasının kod adını alır. |
| [SetCodeName](./setcodename/) | Çalışma sayfasının kod adını alır. |
| [GetBackgroundImage](./getbackgroundimage/) | Çalışma sayfasının arka plan resmini alır ve ayarlar. |
| [SetBackgroundImage](./setbackgroundimage/) | Çalışma sayfasının arka plan resmini alır ve ayarlar. |
| [GetConditionalFormattings](./getconditionalformattings/) | Çalışma sayfasındaki ConditionalFormattings öğesini alır. |
| [GetActiveCell](./getactivecell/) | Çalışma sayfasındaki etkin hücreyi alır veya ayarlar. |
| [SetActiveCell](./setactivecell/) | Çalışma sayfasındaki etkin hücreyi alır veya ayarlar. |
| [GetCustomProperties](./getcustomproperties/) | Çalışma sayfasıyla ilişkili tanımlayıcı bilgilerini temsil eden bir nesneyi alır. |
| [GetPrintingPageBreaks](./getprintingpagebreaks/) | Otomatik sayfa sonlarını alır. |
| [GetSmartTagSetting](./getsmarttagsetting/) | Çalışma sayfasının tüm SmartTagCollection nesnelerini alır. |
| [ToString](./tostring/) | Geçerli Worksheet nesnesini temsil eden bir dize döndürür. |
| [GetScenarios](./getscenarios/) | Scenario koleksiyonunu alır. |
| [StartAccessCache](./startaccesscache/) | Bu çalışma sayfasındaki verilere erişmek için önbellekleri kullanan oturumu başlatır. |
| [CloseAccessCache](./closeaccesscache/) | Bu çalışma sayfasındaki verilere erişmek için önbellekleri kullanan oturumu kapatır. |
| [ConvertFormulaReferenceStyle](./convertformulareferencestyle/) | Formül referans stilini dönüştürür. |
| [CalculateFormula_String](./calculateformula_string/) | Bir formülü hesaplar. |
| [CalculateFormula_String_CalculationOptions](./calculateformula_string_calculationoptions/) | Bir formül ifadesini doğrudan hesaplar. |
| [CalculateFormula_String_FormulaParseOptions_CalculationOptions_Int_Int_CalculationData](./calculateformula_string_formulaparseoptions_calculationoptions_int_int_calculationdata/) | Bir formül ifadesini doğrudan hesaplar. |
| [CalculateArrayFormula_String_CalculationOptions](./calculatearrayformula_string_calculationoptions/) | Formülü dizi formülü olarak hesaplar. |
| [CalculateArrayFormula_String_CalculationOptions_Int_Int](./calculatearrayformula_string_calculationoptions_int_int/) | Formülü dizi formülü olarak hesaplar. |
| [CalculateArrayFormula_String_FormulaParseOptions_CalculationOptions_Int_Int_Int_Int_CalculationData](./calculatearrayformula_string_formulaparseoptions_calculationoptions_int_int_int_int_calculationdata/) | Formülü dizi formülü olarak hesaplar. |
| [CalculateFormula_CalculationOptions_Bool](./calculateformula_calculationoptions_bool/) | Bu çalışma sayfasındaki tüm formülleri hesaplar. |
| [GetAreasOfXmlMapQuery](./getareasofxmlmapquery/) | XML haritasının belirli yoluna eşlenen/bağlanan hücre alanlarını sorgular. |
| [GetCellWatches](./getcellwatches/) | Bu çalışma sayfasında 'watch window' içinde izlenen hücrelerin koleksiyonunu alır. |
| [RefreshPivotTables](./refreshpivottables/) | Bu çalışma sayfasındaki tüm PivotTable'ları yeniler. |
| [RefreshPivotTables_PivotTableRefreshOption](./refreshpivottables_pivottablerefreshoption/) | Bu çalışma sayfasındaki tüm PivotTable'ları yeniler. |
