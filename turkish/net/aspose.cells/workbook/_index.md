---
title: Workbook
second_title: Aspose.Cells for .NET API Referansı
description: Bir Excel elektronik tablosu oluşturmak için bir kök nesneyi temsil eder.
type: docs
weight: 6480
url: /tr/net/aspose.cells/workbook/
---
## Workbook class

Bir Excel elektronik tablosu oluşturmak için bir kök nesneyi temsil eder.

```csharp
public class Workbook : IDisposable
```

## yapıcılar

| İsim | Tanım |
| --- | --- |
| [Workbook](workbook#constructor)() | Yeni bir örneğini başlatır[`Workbook`](../workbook) sınıf. |
| [Workbook](workbook#constructor_1)(FileFormatType) | Yeni bir örneğini başlatır[`Workbook`](../workbook) sınıf. |
| [Workbook](workbook#constructor_2)(Stream) | Yeni bir örneğini başlatır[`Workbook`](../workbook) sınıf ve bir akış açın. |
| [Workbook](workbook#constructor_4)(string) | Yeni bir örneğini başlatır[`Workbook`](../workbook) sınıf ve bir dosya açın. |
| [Workbook](workbook#constructor_3)(Stream, LoadOptions) | Yeni bir örneğini başlatır[`Workbook`](../workbook) sınıf ve açık akış. |
| [Workbook](workbook#constructor_5)(string, LoadOptions) | Yeni bir örneğini başlatır[`Workbook`](../workbook) sınıf ve bir dosya açın. |

## Özellikleri

| İsim | Tanım |
| --- | --- |
| [AbsolutePath](../../aspose.cells/workbook/absolutepath) { get; set; } | Dosyanın mutlak yolunu alır ve ayarlar. |
| [BuiltInDocumentProperties](../../aspose.cells/workbook/builtindocumentproperties) { get; } | Bir döndürür[`DocumentProperty`](../../aspose.cells.properties/documentproperty)elektronik tablonun tüm yerleşik belge özelliklerini temsil eden koleksiyon. |
| [CellsDataTableFactory](../../aspose.cells/workbook/cellsdatatablefactory) { get; } | Özel nesnelerden ICellsDataTable oluşturmak için fabrikayı alır |
| [Colors](../../aspose.cells/workbook/colors) { get; } | Elektronik tablonun paletindeki renkleri döndürür. |
| [ContentTypeProperties](../../aspose.cells/workbook/contenttypeproperties) { get; } | Şunların listesini alır[`ContentTypeProperty`](../../aspose.cells.properties/contenttypeproperty) çalışma kitabındaki nesneler. |
| [CountOfStylesInPool](../../aspose.cells/workbook/countofstylesinpool) { get; } | Stil havuzundaki stillerin sayısını alır. |
| [CustomDocumentProperties](../../aspose.cells/workbook/customdocumentproperties) { get; } | Bir döndürür[`DocumentProperty`](../../aspose.cells.properties/documentproperty) elektronik tablonun tüm özel belge özelliklerini temsil eden koleksiyon. |
| [CustomXmlParts](../../aspose.cells/workbook/customxmlparts) { get; } | Bir Özel XML Veri Depolama Bölümünü temsil eder (bir paket içindeki özel XML verileri). |
| [DataConnections](../../aspose.cells/workbook/dataconnections) { get; } | [`ExternalConnection`](../../aspose.cells.externalconnections/externalconnection) koleksiyon. |
| [DataMashup](../../aspose.cells/workbook/datamashup) { get; } | Karma verileri alır. |
| [DataSorter](../../aspose.cells/workbook/datasorter) { get; } | Verileri sıralamak için bir DataSorter nesnesi alır. |
| [DefaultStyle](../../aspose.cells/workbook/defaultstyle) { get; set; } | Varsayılanı alır veya ayarlar[`Style`](../style) çalışma kitabının nesnesi. |
| [FileFormat](../../aspose.cells/workbook/fileformat) { get; set; } | Dosya biçimini alır ve ayarlar. |
| [FileName](../../aspose.cells/workbook/filename) { get; set; } | Geçerli dosya adını alır ve ayarlar. |
| [HasMacro](../../aspose.cells/workbook/hasmacro) { get; } | Bu elektronik tablonun makro/VBA içerip içermediğini gösterir. |
| [HasRevisions](../../aspose.cells/workbook/hasrevisions) { get; } | Çalışma kitabında izlenen değişiklikler olup olmadığını alır |
| [InterruptMonitor](../../aspose.cells/workbook/interruptmonitor) { get; set; } | Kesinti izleyicisini alır ve ayarlar. |
| [IsDigitallySigned](../../aspose.cells/workbook/isdigitallysigned) { get; } | Bu e-tablonun dijital olarak imzalanıp imzalanmadığını gösterir. |
| [IsLicensed](../../aspose.cells/workbook/islicensed) { get; } | Lisansın ayarlanıp ayarlanmadığını gösterir. |
| [IsWorkbookProtectedWithPassword](../../aspose.cells/workbook/isworkbookprotectedwithpassword) { get; } | Yapının veya pencerenin parola ile korunup korunmadığını belirtir. |
| [RibbonXml](../../aspose.cells/workbook/ribbonxml) { get; set; } | Şerit Kullanıcı Arabirimini tanımlayan XML dosyasını alır ve ayarlar. |
| [Settings](../../aspose.cells/workbook/settings) { get; } | Çalışma kitabı ayarlarını temsil eder. |
| [Theme](../../aspose.cells/workbook/theme) { get; } | Tema adını alır. |
| [VbaProject](../../aspose.cells/workbook/vbaproject) { get; } | [`VbaProject`](./vbaproject) bir elektronik tabloda. |
| [Worksheets](../../aspose.cells/workbook/worksheets) { get; } | [`WorksheetCollection`](../worksheetcollection) elektronik tabloda toplama. |

## yöntemler

| İsim | Tanım |
| --- | --- |
| [AcceptAllRevisions](../../aspose.cells/workbook/acceptallrevisions)() | Çalışma kitabında izlenen tüm değişiklikleri kabul eder. |
| [AddDigitalSignature](../../aspose.cells/workbook/adddigitalsignature)(DigitalSignatureCollection) | Bir OOXML elektronik tablo dosyasına dijital imza ekler (Excel2007 ve sonrası). |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula)() | Formüllerin sonucunu hesaplar. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula_2)(bool) | Formüllerin sonucunu hesaplar. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula#calculateformula_1)(CalculationOptions) | Bu çalışma kitabındaki formülleri hesaplama. |
| [ChangePalette](../../aspose.cells/workbook/changepalette)(Color, int) | Belirtilen dizindeki elektronik tablonun paletini değiştirir. |
| [CloseAccessCache](../../aspose.cells/workbook/closeaccesscache)(AccessCacheOptions) | Verilere erişmek için önbellek kullanan oturumu kapatır. |
| [Combine](../../aspose.cells/workbook/combine)(Workbook) | Başka bir Çalışma Kitabı nesnesini birleştirir. |
| [Copy](../../aspose.cells/workbook/copy#copy)(Workbook) | Kaynak Çalışma Kitabı nesnesindeki verileri kopyalar. |
| [Copy](../../aspose.cells/workbook/copy#copy_1)(Workbook, CopyOptions) | Kaynak Çalışma Kitabı nesnesindeki verileri kopyalar. |
| [CopyTheme](../../aspose.cells/workbook/copytheme)(Workbook) | Temayı başka bir çalışma kitabından kopyalar. |
| [CreateBuiltinStyle](../../aspose.cells/workbook/createbuiltinstyle)(BuiltinStyleType) | Verilen türe göre yerleşik stil oluşturur. |
| [CreateCellsColor](../../aspose.cells/workbook/createcellscolor)() | Bir[`CellsColor`](../cellscolor) nesne. |
| [CreateStyle](../../aspose.cells/workbook/createstyle)() | Yeni bir stil oluşturur. |
| [CustomTheme](../../aspose.cells/workbook/customtheme)(string, Color[]) | Temayı özelleştirir. |
| [Dispose](../../aspose.cells/workbook/dispose)() | Yönetilmeyen kaynakları serbest bırakma, serbest bırakma veya sıfırlama ile ilişkili uygulama tanımlı görevleri gerçekleştirir. |
| [ExportXml](../../aspose.cells/workbook/exportxml#exportxml)(string, Stream) | XML verilerini dışa aktarın. |
| [ExportXml](../../aspose.cells/workbook/exportxml#exportxml_1)(string, string) | Belirtilen XML haritasıyla bağlantılı XML verilerini dışa aktarın. |
| [GetDigitalSignature](../../aspose.cells/workbook/getdigitalsignature)() | Dosyadan dijital imza alır. |
| [GetFonts](../../aspose.cells/workbook/getfonts)() | Stil havuzundaki tüm yazı tiplerini alır. |
| [GetMatchingColor](../../aspose.cells/workbook/getmatchingcolor)(Color) | Geçerli palette en uygun Rengi bulun. |
| [GetNamedStyle](../../aspose.cells/workbook/getnamedstyle)(string) | Stil havuzunda adlandırılmış stili alır. |
| [GetStyleInPool](../../aspose.cells/workbook/getstyleinpool)(int) | Stil havuzundaki stili alır. Çalışma kitabındaki tüm stiller bir havuzda toplanacaktır. Hücrelerde yalnızca basit bir başvuru dizini vardır. |
| [GetThemeColor](../../aspose.cells/workbook/getthemecolor)(ThemeColorType) | Tema rengini alır. |
| [ImportXml](../../aspose.cells/workbook/importxml#importxml)(Stream, string, int, int) | Bir XML veri dosyasını çalışma kitabına aktarır/günceller. |
| [ImportXml](../../aspose.cells/workbook/importxml#importxml_1)(string, string, int, int) | Bir XML veri dosyasını çalışma kitabına aktarır/günceller. |
| [IsColorInPalette](../../aspose.cells/workbook/iscolorinpalette)(Color) | Elektronik tablonun paletinde bir renk olup olmadığını kontrol eder. |
| [ParseFormulas](../../aspose.cells/workbook/parseformulas)(bool) | Şablon dosyasından yüklendiğinde veya bir hücreye ayarlandığında ayrıştırılmamış tüm formülleri ayrıştırır. |
| [Protect](../../aspose.cells/workbook/protect)(ProtectionType, string) | Çalışma kitabını korur. |
| [ProtectSharedWorkbook](../../aspose.cells/workbook/protectsharedworkbook)(string) | Paylaşılan bir çalışma kitabını korur. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas)(bool) | Dinamik dizi formüllerini yeniler (geçerli verilere göre yeni komşu hücre aralığına dökülür) |
| [RemoveDigitalSignature](../../aspose.cells/workbook/removedigitalsignature)() | Bu elektronik tablodan dijital imzayı kaldırır. |
| [RemoveMacro](../../aspose.cells/workbook/removemacro)() | Bu e-tablodan VBA/makroyu kaldırır. |
| [RemovePersonalInformation](../../aspose.cells/workbook/removepersonalinformation)() | Kişisel bilgileri kaldırır. |
| [RemoveUnusedStyles](../../aspose.cells/workbook/removeunusedstyles)() | Kullanılmayan tüm stilleri kaldırın. |
| [Replace](../../aspose.cells/workbook/replace#replace)(bool, object) | Hücrelerin değerlerini yeni verilerle değiştirir. |
| [Replace](../../aspose.cells/workbook/replace#replace_1)(int, object) | Hücrelerin değerlerini yeni verilerle değiştirir. |
| [Replace](../../aspose.cells/workbook/replace#replace_6)(string, DataTable) | Hücrelerin değerlerini birDataTable . |
| [Replace](../../aspose.cells/workbook/replace#replace_2)(string, double) | Bir hücrenin değerini yeni bir double ile değiştirir. |
| [Replace](../../aspose.cells/workbook/replace#replace_4)(string, int) | Bir hücrenin değerini yeni bir tamsayı ile değiştirir. |
| [Replace](../../aspose.cells/workbook/replace#replace_7)(string, string) | Bir hücrenin değerini yeni bir dizeyle değiştirir. |
| [Replace](../../aspose.cells/workbook/replace#replace_3)(string, double[], bool) | Hücrelerin değerlerini bir çift diziyle değiştirir. |
| [Replace](../../aspose.cells/workbook/replace#replace_5)(string, int[], bool) | Hücrelerin değerlerini bir tamsayı dizisiyle değiştirir. |
| [Replace](../../aspose.cells/workbook/replace#replace_8)(string, string, ReplaceOptions) | Bir hücrenin değerini yeni bir dizeyle değiştirir. |
| [Replace](../../aspose.cells/workbook/replace#replace_9)(string, string[], bool) | Bir hücrenin değerini yeni bir dize dizisiyle değiştirir. |
| [Save](../../aspose.cells/workbook/save#save_2)(string) | Çalışma kitabını diske kaydedin. |
| [Save](../../aspose.cells/workbook/save#save)(Stream, SaveFormat) | Çalışma kitabını akışa kaydeder. |
| [Save](../../aspose.cells/workbook/save#save_1)(Stream, SaveOptions) | Çalışma kitabını akışa kaydeder. |
| [Save](../../aspose.cells/workbook/save#save_3)(string, SaveFormat) | Çalışma kitabını diske kaydeder. |
| [Save](../../aspose.cells/workbook/save#save_4)(string, SaveOptions) | Çalışma kitabını diske kaydeder. |
| [Save](../../aspose.cells/workbook/save#save_5)(HttpResponse, string, ContentDisposition, SaveOptions) | Sonuç elektronik tablosunu oluşturur ve istemciye aktarır, ardından tarayıcıda veya MS Workbook'ta açar. |
| [Save](../../aspose.cells/workbook/save#save_6)(HttpResponse, string, ContentDisposition, SaveOptions, bool) | Sonuç elektronik tablosunu oluşturur ve istemciye aktarır, ardından tarayıcıda veya MS Workbook'ta açar. |
| [SaveToStream](../../aspose.cells/workbook/savetostream)() | Excel dosyasını bir MemoryStream nesnesine kaydeder ve onu döndürür. |
| [SetDigitalSignature](../../aspose.cells/workbook/setdigitalsignature)(DigitalSignatureCollection) | Dijital imzayı bir elektronik tablo dosyasına ayarlar (Excel2007 ve üstü). |
| [SetEncryptionOptions](../../aspose.cells/workbook/setencryptionoptions)(EncryptionType, int) | Şifreleme Seçeneklerini Ayarlayın. |
| [SetThemeColor](../../aspose.cells/workbook/setthemecolor)(ThemeColorType, Color) | color temasını ayarlar |
| [StartAccessCache](../../aspose.cells/workbook/startaccesscache)(AccessCacheOptions) | Verilere erişmek için önbellek kullanan oturumu başlatır. |
| [Unprotect](../../aspose.cells/workbook/unprotect)(string) | Çalışma kitabının korumasını kaldırır. |
| [UnprotectSharedWorkbook](../../aspose.cells/workbook/unprotectsharedworkbook)(string) | Paylaşılan bir çalışma kitabının korumasını kaldırır. |
| [UpdateLinkedDataSource](../../aspose.cells/workbook/updatelinkeddatasource)(Workbook[]) | Bu çalışma kitabı başka bir veri kaynağına harici bağlantılar içeriyorsa, Aspose.Cells en son verileri almaya çalışır. |

### Notlar

Çalışma Kitabı sınıfı, bir Excel elektronik tablosunu belirtir. Her elektronik tablo birden çok çalışma sayfası içerebilir. Sınıfın temel özelliği, yerel excel dosyalarını açmak ve kaydetmektir. Sınıf, diğer Çalışma Kitaplarından veri kopyalama, iki Çalışma Kitabını birleştirme ve Excel elektronik tablosunu koruma gibi bazı gelişmiş özelliklere sahiptir.

### Örnekler

Aşağıdaki örnek, design.xls adlı bir dosyadan bir Çalışma Kitabı yükler ve yatay ve dikey kaydırma çubuklarını Çalışma Kitabı için görünmez kılar. Ardından, elektronik tablodaki iki dize değerini sırasıyla bir Tamsayı değeri ve dize değeriyle değiştirir ve son olarak güncellenen dosyayı istemci tarayıcısına gönderir.

```csharp
[C#]

//Bir tasarımcı dosyası aç
string designerFile = "designer.xls";
Workbook workbook = new Workbook(designerFile);

//Kaydırma çubuklarını ayarla
workbook.Settings.IsHScrollBarVisible = false;
workbook.Settings.IsVScrollBarVisible = false;

//yer tutucu dizeyi yeni değerlerle değiştir
int newInt = 100;
workbook.Replace("OldInt", newInt);

string newString = "Hello!";
workbook.Replace("OldString", newString);
workbook.Save("result.xls");

[Visual Basic]

'Bir tasarımcı dosyası açın
Dim designerFile as String = "\designer.xls"
Dim workbook as Workbook = new Workbook(designerFile)

'Kaydırma çubuklarını ayarla
workbook.IsHScrollBarVisible = False
workbook.IsVScrollBarVisible = False

'Yer tutucu dizesini yeni değerlerle değiştirin
Dim newInt as Integer = 100
workbook.Replace("OldInt", newInt)

Dim newString as String = "Hello!"
workbook.Replace("OldString", newString)
workbook.Save("result.xls")    
```

### Ayrıca bakınız

* ad alanı [Aspose.Cells](../../aspose.cells)
* toplantı [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
