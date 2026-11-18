---
title: "Workbook Sınıfı"
linktitle: "Workbook"
second_title: "C++ API Referansı aracılığıyla Go için Aspose.Cells"
description: "Workbook sınıfı. Go dilinde workbook'u temsil eden nesneyi kapsüller."
type: docs
weight: 200
url: /tr/go-cpp/workbook/
---

## Workbook class

Excel çalışma sayfası oluşturmak için bir kök nesneyi temsil eder.

```go

type Workbook struct  {
	ptr unsafe.Pointer
}

```
## Yapıcılar

| Metot | Açıklama |
| --- | --- |
| [NewWorkbook](./newworkbook/) | Workbook sınıfının yeni bir örneğini başlatır. |
| [NewWorkbook_FileFormatType](./newworkbook_fileformattype/) | Workbook sınıfının yeni bir örneğini başlatır. |
| [NewWorkbook_LoadOptions](./newworkbook_loadoptions/) | Seçeneklerle Workbook sınıfının yeni boş bir örneğini başlatır |
| [NewWorkbook_String](./newworkbook_string/) | Workbook sınıfının yeni bir örneğini başlatır ve bir dosya açar. |
| [NewWorkbook_Stream](./newworkbook_stream/) | Workbook sınıfının yeni bir örneğini başlatır ve bir akış açar. |
| [NewWorkbook_String_LoadOptions](./newworkbook_string_loadoptions/) | Workbook sınıfının yeni bir örneğini başlatır ve bir dosya açar. |
| [NewWorkbook_Stream_LoadOptions](./newworkbook_stream_loadoptions/) | Workbook sınıfının yeni bir örneğini başlatır ve akışı açar. |

## Metotlar

| Metot | Açıklama |
| --- | --- |
| [IsNull](./isnull/) | Uygulama nesnesinin nullptr olup olmadığını kontrol eder. |
| [GetSettings](./getsettings/) | Workbook ayarlarını temsil eder. |
| [ParseFormulas](./parseformulas/) | Şablon dosyasından yüklendiğinde veya bir hücreye ayarlandığında henüz ayrıştırılmamış tüm formülleri ayrıştırır. |
| [StartAccessCache](./startaccesscache/) | Veriye erişmek için önbellekleri kullanan oturumu başlatır. |
| [CloseAccessCache](./closeaccesscache/) | Önbellekleri kullanarak veri erişen oturumu kapatır. |
| [Save_String_SaveFormat](./save_string_saveformat/) | Çalışma kitabını diske kaydeder. |
| [Save_String](./save_string/) | Çalışma kitabını diske kaydet. |
| [Save_String_SaveOptions](./save_string_saveoptions/) | Çalışma kitabını diske kaydeder. |
| [Save_SaveFormat](./save_saveformat/) | Çalışma kitabını akışa kaydeder. |
| [Save_SaveOptions](./save_saveoptions/) | Çalışma kitabını akışa kaydeder. |
| [SaveToStream](./savetostream/) | Excel dosyasını bir MemoryStream nesnesine Excel97-2003 xls dosyası olarak kaydeder ve döndürür. |
| [GetWorksheets](./getworksheets/) | Elektronik tablo içindeki WorksheetCollection koleksiyonunu alır. |
| [IsLicensed](./islicensed/) | Lisansın ayarlanıp ayarlanmadığını gösterir. |
| [RemoveUnusedStyles](./removeunusedstyles/) | Kullanılmayan tüm stilleri kaldırır. |
| [CreateStyle](./createstyle/) | Yeni bir stil oluşturur. |
| [CreateStyle_Bool](./createstyle_bool/) | Yeni bir stil oluşturur. |
| [CreateBuiltinStyle](./createbuiltinstyle/) | Verilen tipe göre yerleşik stil oluşturur. |
| [CreateCellsColor](./createcellscolor/) | Bir CellsColor nesnesi oluşturur. |
| [Replace_String_String](./replace_string_string/) | Bir hücrenin değerini yeni bir dizeyle değiştirir. |
| [Replace_String_Int](./replace_string_int/) | Bir hücrenin değerini yeni bir tam sayı ile değiştirir. |
| [Replace_String_Double](./replace_string_double/) | Bir hücrenin değerini yeni bir double ile değiştirir. |
| [Replace_String_stringArray_Bool](./replace_string_stringarray_bool/) | Bir hücrenin değerini yeni bir dize dizisiyle değiştirir. |
| [Replace_String_int32Array_Bool](./replace_string_int32array_bool/) | Hücrelerin değerlerini bir tam sayı dizisiyle değiştirir. |
| [Replace_String_float64Array_Bool](./replace_string_float64array_bool/) | Hücrelerin değerlerini bir double dizisiyle değiştirir. |
| [Replace_Bool_Object](./replace_bool_object/) | Hücrelerin değerlerini yeni veriyle değiştirir. |
| [Replace_Int_Object](./replace_int_object/) | Hücrelerin değerlerini yeni veriyle değiştirir. |
| [Replace_String_String_ReplaceOptions](./replace_string_string_replaceoptions/) | Bir hücrenin değerini yeni bir dizeyle değiştirir. |
| [Copy_Workbook_CopyOptions](./copy_workbook_copyoptions/) | Başka bir Workbook nesnesini kopyalar. |
| [Copy_Workbook](./copy_workbook/) | Kaynak bir Workbook nesnesinden verileri kopyalar. |
| [Combine](./combine/) | Başka bir Workbook nesnesini birleştirir. |
| [GetColors](./getcolors/) | Elektronik tablo için palet içindeki renkleri döndürür. |
| [GetStyleInPool](./getstyleinpool/) | Stil havuzundaki stili alır.Tüm stiller çalışma kitabında bir havuza toplanır.Hücrelerde yalnızca basit bir referans indeksi bulunur. |
| [GetCountOfStylesInPool](./getcountofstylesinpool/) | Stil havuzundaki stil sayısını alır. |
| [GetFonts](./getfonts/) | Stil havuzundaki tüm yazı tiplerini alır. |
| [GetNamedStyle](./getnamedstyle/) | Stil havuzundaki adlandırılmış stili alır. |
| [MergeNamedStyles](./mergenamedstyles/) | Diğer Excel dosyasından adlandırılmış stilleri birleştirir. |
| [ChangePalette](./changepalette/) | Belirtilen indeksteki elektronik tablo için paleti değiştirir. |
| [IsColorInPalette](./iscolorinpalette/) | Elektronik tablo için palette bir rengin olup olmadığını kontrol eder. |
| [CalculateFormula](./calculateformula/) | Formüllerin sonucunu hesaplar. |
| [CalculateFormula_Bool](./calculateformula_bool/) | Formüllerin sonucunu hesaplar. |
| [CalculateFormula_CalculationOptions](./calculateformula_calculationoptions/) | Bu çalışma kitabındaki formüller hesaplanıyor. |
| [RefreshDynamicArrayFormulas_Bool](./refreshdynamicarrayformulas_bool/) | Dinamik dizi formüllerini yeniler (geçerli verilere göre komşu hücrelerin yeni bir aralığına yayılır). Çalışma kitabındaki diğer formüller, dinamik dizi formülleri tarafından kullanılsa bile, yinelemeli olarak hesaplanmayacaktır. |
| [RefreshDynamicArrayFormulas_Bool_CalculationOptions](./refreshdynamicarrayformulas_bool_calculationoptions/) | Dinamik dizi formüllerini yeniler (geçerli verilere göre komşu hücrelerin yeni bir aralığına yayılır). |
| [GetDefaultStyle](./getdefaultstyle/) | Çalışma kitabının varsayılan Style nesnesini alır veya ayarlar. |
| [SetDefaultStyle](./setdefaultstyle/) | Çalışma kitabının varsayılan Style nesnesini alır veya ayarlar. |
| [GetMatchingColor](./getmatchingcolor/) | Mevcut palet içinde en uygun eşleşen Color'ı bul. |
| [IsDigitallySigned](./isdigitallysigned/) | Bu elektronik tablonun dijital olarak imzalı olup olmadığını gösterir. |
| [SetEncryptionOptions](./setencryptionoptions/) | Şifreleme seçeneklerini ayarla. |
| [Protect](./protect/) | Bir çalışma kitabını korur. |
| [ProtectSharedWorkbook](./protectsharedworkbook/) | Paylaşılan bir çalışma kitabını korur. |
| [Unprotect](./unprotect/) | Bir çalışma kitabının korumasını kaldırır. |
| [UnprotectSharedWorkbook](./unprotectsharedworkbook/) | Paylaşılan bir çalışma kitabının korumasını kaldırır. |
| [IsWorkbookProtectedWithPassword](./isworkbookprotectedwithpassword/) | Yapının veya pencerenin parola ile korunup korunmadığını gösterir. |
| [RemoveMacro](./removemacro/) | Bu elektronik tablodan VBA/makroyu kaldırır. |
| [GetVbaProject](./getvbaproject/) | Bir elektronik tablodaki VbaProject'i alır. |
| [RemoveDigitalSignature](./removedigitalsignature/) | Bu elektronik tablodan dijital imzayı kaldırır. |
| [AcceptAllRevisions](./acceptallrevisions/) | Çalışma kitabındaki tüm izlenen değişiklikleri kabul eder. |
| [GetHasMacro](./gethasmacro/) | Bu elektronik tablonun makro/VBA içerip içermediğini gösterir. |
| [GetHasRevisions](./gethasrevisions/) | Çalışma kitabının izlenen değişiklikleri olup olmadığını alır. |
| [GetFileName](./getfilename/) | Geçerli dosya adını alır ve ayarlar. |
| [SetFileName](./setfilename/) | Geçerli dosya adını alır ve ayarlar. |
| [GetDataSorter](./getdatasorter/) | Verileri sıralamak için bir DataSorter nesnesi alır. |
| [GetThemeColor](./getthemecolor/) | Tema rengini alır. |
| [SetThemeColor](./setthemecolor/) | Tema rengini ayarlar |
| [GetTheme](./gettheme/) | Tema adını alır. |
| [CustomTheme](./customtheme/) | Temayı özelleştirir. |
| [CopyTheme](./copytheme/) | Temayı başka bir çalışma kitabından kopyalar. |
| [UpdateCustomFunctionDefinition](./updatecustomfunctiondefinition/) | Özel işlevlerin tanımını günceller. |
| [UpdateLinkedDataSource](./updatelinkeddatasource/) | Bu çalışma kitabı diğer veri kaynaklarına dış bağlantılar içeriyorsa,Aspose.Cells verilen kaynaklardan en son verileri almaya çalışacaktır. |
| [GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | Elektronik tabloyun tüm yerleşik belge özelliklerini temsil eden bir DocumentProperty koleksiyonu döndürür. |
| [GetCustomDocumentProperties](./getcustomdocumentproperties/) | Elektronik tabloyun tüm özel belge özelliklerini temsil eden bir DocumentProperty koleksiyonu döndürür. |
| [GetFileFormat](./getfileformat/) | Dosya biçimini alır ve ayarlar. |
| [SetFileFormat](./setfileformat/) | Dosya biçimini alır ve ayarlar. |
| [GetHasCustomFunction](./gethascustomfunction/) | Bu çalışma kitabında hücre formüllerinde, tanımlı adlarda vb. kullanılan özel işlevlerin olup olmadığını algılar... |
| [GetInterruptMonitor](./getinterruptmonitor/) | Kesinti izleyicisini alır ve ayarlar. |
| [SetInterruptMonitor_AbstractInterruptMonitor](./setinterruptmonitor_abstractinterruptmonitor/) | Kesinti izleyicisini alır ve ayarlar. |
| [SetInterruptMonitor_InterruptMonitor](./setinterruptmonitor_interruptmonitor/) | Kesinti izleyicisini ayarlar. |
| [GetContentTypeProperties](./getcontenttypeproperties/) | Çalışma kitabındaki ContentTypeProperty nesnelerinin listesini alır. |
| [GetCustomXmlParts](./getcustomxmlparts/) | Özel XML Veri Depolama Bölümünü (paket içindeki özel XML verisi) temsil eder. |
| [GetDataMashup](./getdatamashup/) | Birleştirme verilerini alır. |
| [GetRibbonXml](./getribbonxml/) | Ribbon UI'yi tanımlayan XML dosyasını alır ve ayarlar. |
| [SetRibbonXml](./setribbonxml/) | Ribbon UI'yi tanımlayan XML dosyasını alır ve ayarlar. |
| [GetAbsolutePath](./getabsolutepath/) | Dosyanın mutlak yolunu alır ve ayarlar. |
| [SetAbsolutePath](./setabsolutepath/) | Dosyanın mutlak yolunu alır ve ayarlar. |
| [GetDataConnections](./getdataconnections/) | ExternalConnection koleksiyonunu alır. |
| [ImportXml_String_String_Int_Int](./importxml_string_string_int_int/) | Bir XML veri dosyasını çalışma kitabına içe aktarır/günceller. |
| [ImportXml_Stream_String_Int_Int](./importxml_stream_string_int_int/) | Bir XML veri dosyasını çalışma kitabına içe aktarır/günceller. |
| [ExportXml_String_String](./exportxml_string_string/) | Belirtilen XML haritası ile bağlantılı XML verilerini dışa aktar. |
| [ExportXml_String](./exportxml_string/) | XML verilerini dışa aktar. |
| [SetDigitalSignature](./setdigitalsignature/) | Bir elektronik tablo dosyasına (Excel2007 ve sonrası) dijital imza ekler. |
| [AddDigitalSignature](./adddigitalsignature/) | OOXML elektronik tablo dosyasına (Excel2007 ve sonrası) dijital imza ekler. |
| [GetDigitalSignature](./getdigitalsignature/) | Dosyadan dijital imzayı alır. |
| [RemovePersonalInformation](./removepersonalinformation/) | Kişisel bilgileri kaldırır. |
| [GetDataModel](./getdatamodel/) | Çalışma kitabındaki veri modelini alır. |
| [RefreshAll](./refreshall/) | Bağlantılı şekilleri, tüm pivot tabloları ve pivot kaynağına sahip grafikleri yenileyin. |
| [Dispose](./dispose/) | Yönetilmeyen kaynakları serbest bırakma, bırakma veya sıfırlama ile ilgili uygulama tanımlı görevleri yürütür. |
