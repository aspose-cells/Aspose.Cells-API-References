---
title: "Sınıf Workbook"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.Workbook class. Excel elektronik tablosu oluşturmak için bir kök nesneyi temsil eder"
type: docs
url: /tr/net/aspose.cells/workbook/
---
## Workbook class

Excel çalışma sayfası oluşturmak için bir kök nesneyi temsil eder.

```csharp
public class Workbook : IDisposable
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Workbook](workbook/#constructor)() | `Workbook` sınıfının yeni bir örneğini başlatır. |
| [Workbook](workbook/#constructor_1)(FileFormatType) | `Workbook` sınıfının yeni bir örneğini başlatır. |
| [Workbook](workbook/#constructor_2)(LoadOptions) | `Workbook` sınıfının seçeneklerle yeni boş bir örneğini başlatır |
| [Workbook](workbook/#constructor_3)(Stream) | `Workbook` sınıfının yeni bir örneğini başlatır ve bir akış açar. |
| [Workbook](workbook/#constructor_5)(string) | `Workbook` sınıfının yeni bir örneğini başlatır ve bir dosya açar. |
| [Workbook](workbook/#constructor_4)(Stream, LoadOptions) | Yeni bir `Workbook` sınıfı örneği başlatır ve akışı açar. |
| [Workbook](workbook/#constructor_6)(string, LoadOptions) | `Workbook` sınıfının yeni bir örneğini başlatır ve bir dosya açar. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AbsolutePath](../../aspose.cells/workbook/absolutepath/) { get; set; } | Dosyanın mutlak yolunu alır ve ayarlar. |
| [BuiltInDocumentProperties](../../aspose.cells/workbook/builtindocumentproperties/) { get; } | Elektronik tablonun tüm yerleşik belge özelliklerini temsil eden bir [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) koleksiyonu döndürür. |
| [CellsDataTableFactory](../../aspose.cells/workbook/cellsdatatablefactory/) { get; } | Özel nesnelerden ICellsDataTable oluşturmak için fabrikayı alır. |
| [Colors](../../aspose.cells/workbook/colors/) { get; } | Elektronik tablo için palet içindeki renkleri döndürür. |
| [ContentTypeProperties](../../aspose.cells/workbook/contenttypeproperties/) { get; } | Çalışma kitabındaki [`ContentTypeProperty`](../../aspose.cells.properties/contenttypeproperty/) nesnelerinin listesini alır. |
| [CountOfStylesInPool](../../aspose.cells/workbook/countofstylesinpool/) { get; } | Stil havuzundaki stil sayısını alır. |
| [CustomDocumentProperties](../../aspose.cells/workbook/customdocumentproperties/) { get; } | Elektronik tablonun tüm özel belge özelliklerini temsil eden bir [`DocumentProperty`](../../aspose.cells.properties/documentproperty/) koleksiyonu döndürür. |
| [CustomXmlParts](../../aspose.cells/workbook/customxmlparts/) { get; } | Özel bir XML Veri Depolama Bölümünü (paket içindeki özel XML verisi) temsil eder. |
| [DataConnections](../../aspose.cells/workbook/dataconnections/) { get; } | [`ExternalConnection`](../../aspose.cells.externalconnections/externalconnection/) koleksiyonunu alır. |
| [DataMashup](../../aspose.cells/workbook/datamashup/) { get; } | Karışım verilerini alır. |
| [DataModel](../../aspose.cells/workbook/datamodel/) { get; } | Çalışma kitabındaki veri modelini alır. |
| [DataSorter](../../aspose.cells/workbook/datasorter/) { get; } | Verileri sıralamak için bir DataSorter nesnesi alır. |
| [DefaultStyle](../../aspose.cells/workbook/defaultstyle/) { get; set; } | Çalışma kitabının varsayılan [`Style`](../style/) nesnesini alır veya ayarlar. |
| [FileFormat](../../aspose.cells/workbook/fileformat/) { get; set; } | Dosya biçimini alır ve ayarlar. |
| [FileName](../../aspose.cells/workbook/filename/) { get; set; } | Geçerli dosya adını alır ve ayarlar. |
| [HasCustomFunction](../../aspose.cells/workbook/hascustomfunction/) { get; } | Bu çalışma kitabında, hücre formüllerinde veya tanımlı adlarda kullanılan özel işlevlerin olup olmadığını algılar... |
| [HasMacro](../../aspose.cells/workbook/hasmacro/) { get; } | Bu elektronik tablonun makro/VBA içerip içermediğini gösterir. |
| [HasRevisions](../../aspose.cells/workbook/hasrevisions/) { get; } | Çalışma kitabının izlenen değişiklikleri olup olmadığını alır. |
| [InterruptMonitor](../../aspose.cells/workbook/interruptmonitor/) { get; set; } | Kesinti izleyicisini alır ve ayarlar. |
| [IsDigitallySigned](../../aspose.cells/workbook/isdigitallysigned/) { get; } | Bu elektronik tablonun dijital olarak imzalı olup olmadığını gösterir. |
| [IsLicensed](../../aspose.cells/workbook/islicensed/) { get; } | Lisansın ayarlanıp ayarlanmadığını gösterir. |
| [IsWorkbookProtectedWithPassword](../../aspose.cells/workbook/isworkbookprotectedwithpassword/) { get; } | Yapının veya pencerenin parola ile korunup korunmadığını gösterir. |
| [RibbonXml](../../aspose.cells/workbook/ribbonxml/) { get; set; } | Ribbon UI'yi tanımlayan XML dosyasını alır ve ayarlar. |
| [Settings](../../aspose.cells/workbook/settings/) { get; } | Çalışma kitabı ayarlarını temsil eder. |
| [Theme](../../aspose.cells/workbook/theme/) { get; } | Tema adını alır. |
| [VbaProject](../../aspose.cells/workbook/vbaproject/) { get; } | Bir elektronik tablodaki [`VbaProject`](./vbaproject/) nesnesini alır. |
| [Worksheets](../../aspose.cells/workbook/worksheets/) { get; } | Elektronik tablodaki [`WorksheetCollection`](../worksheetcollection/) koleksiyonunu alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [AcceptAllRevisions](../../aspose.cells/workbook/acceptallrevisions/)() | Çalışma kitabındaki tüm izlenen değişiklikleri kabul eder. |
| [AddDigitalSignature](../../aspose.cells/workbook/adddigitalsignature/)(DigitalSignatureCollection) | OOXML elektronik tablo dosyasına (Excel2007 ve sonrası) dijital imza ekler. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula)() | Formüllerin sonucunu hesaplar. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula_2)(bool) | Formüllerin sonucunu hesaplar. |
| [CalculateFormula](../../aspose.cells/workbook/calculateformula/#calculateformula_1)(CalculationOptions) | Bu çalışma kitabındaki formüller hesaplanıyor. |
| [ChangePalette](../../aspose.cells/workbook/changepalette/)(Color, int) | Belirtilen indeksteki elektronik tablo için paleti değiştirir. |
| [CloseAccessCache](../../aspose.cells/workbook/closeaccesscache/)(AccessCacheOptions) | Veriye erişmek için önbellekleri kullanan oturumu kapatır. |
| [Combine](../../aspose.cells/workbook/combine/)(Workbook) | Başka bir Workbook nesnesiyle birleştirir. |
| [Copy](../../aspose.cells/workbook/copy/#copy)(Workbook) | Kaynak bir Workbook nesnesinden verileri kopyalar. |
| [Copy](../../aspose.cells/workbook/copy/#copy_1)(Workbook, CopyOptions) | Başka bir Workbook nesnesini kopyalar. |
| [CopyTheme](../../aspose.cells/workbook/copytheme/)(Workbook) | Başka bir çalışma kitabından temayı kopyalar. |
| [CreateBuiltinStyle](../../aspose.cells/workbook/createbuiltinstyle/)(BuiltinStyleType) | Verilen tipe göre yerleşik stil oluşturur. |
| [CreateCellsColor](../../aspose.cells/workbook/createcellscolor/)() | Bir [`CellsColor`](../cellscolor/) nesnesi oluşturur. |
| [CreateStyle](../../aspose.cells/workbook/createstyle/#createstyle)() | Yeni bir stil oluşturur. |
| [CreateStyle](../../aspose.cells/workbook/createstyle/#createstyle_1)(bool) | Yeni bir stil oluşturur. |
| [CustomTheme](../../aspose.cells/workbook/customtheme/)(string, Color[]) | Temayı özelleştirir. |
| [Dispose](../../aspose.cells/workbook/dispose/)() | Yönetilmeyen kaynakların serbest bırakılması, salınması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür. |
| [ExportXml](../../aspose.cells/workbook/exportxml/#exportxml)(string, Stream) | XML verisini dışa aktar. |
| [ExportXml](../../aspose.cells/workbook/exportxml/#exportxml_1)(string, string) | Belirtilen XML haritası ile bağlanmış XML verisini dışa aktar. |
| [GetDigitalSignature](../../aspose.cells/workbook/getdigitalsignature/)() | Dosyadan dijital imzayı alır. |
| [GetFonts](../../aspose.cells/workbook/getfonts/)() | Stil havuzundaki tüm yazı tiplerini alır. |
| [GetMatchingColor](../../aspose.cells/workbook/getmatchingcolor/)(Color) | Mevcut palet içinde en iyi eşleşen Rengi bul. |
| [GetNamedStyle](../../aspose.cells/workbook/getnamedstyle/)(string) | Stil havuzundaki adlandırılmış stili alır. |
| [GetStyleInPool](../../aspose.cells/workbook/getstyleinpool/)(int) | Stil havuzundaki stili alır. Çalışma kitabındaki tüm stiller bir havuza toplanacaktır. Hücrelerde yalnızca basit bir referans indeksi bulunur. |
| [GetThemeColor](../../aspose.cells/workbook/getthemecolor/)(ThemeColorType) | Tema rengini alır. |
| [HasExernalLinks](../../aspose.cells/workbook/hasexernallinks/)() | (**Obsolete.**) Bu çalışma kitabının diğer veri kaynaklarına dış bağlantılar içerip içermediğini gösterir. |
| [ImportXml](../../aspose.cells/workbook/importxml/#importxml)(Stream, string, int, int) | Bir XML veri dosyasını çalışma kitabına içe aktarır/günceller. |
| [ImportXml](../../aspose.cells/workbook/importxml/#importxml_1)(string, string, int, int) | Bir XML veri dosyasını çalışma kitabına içe aktarır/günceller. |
| [IsColorInPalette](../../aspose.cells/workbook/iscolorinpalette/)(Color) | Bir rengin elektronik tablo paletinde olup olmadığını kontrol eder. |
| [MergeNamedStyles](../../aspose.cells/workbook/mergenamedstyles/)(Workbook) | Diğer Excel dosyasından adlandırılmış stilleri birleştirir. |
| [ParseFormulas](../../aspose.cells/workbook/parseformulas/)(bool) | Şablon dosyasından yüklendiğinde veya bir hücreye ayarlandığında ayrılmamış tüm formülleri ayrıştırır. |
| [Protect](../../aspose.cells/workbook/protect/)(ProtectionType, string) | Bir çalışma kitabını korur. |
| [ProtectSharedWorkbook](../../aspose.cells/workbook/protectsharedworkbook/)(string) | Paylaşılan bir çalışma kitabını korur. |
| [RefreshAll](../../aspose.cells/workbook/refreshall/)() | Bağlantılı şekilleri, tüm pivot tablolarını ve pivot kaynağına sahip grafikleri yeniler. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas/#refreshdynamicarrayformulas)(bool) | Dinamik dizi formüllerini (mevcut verilere göre komşu hücrelerin yeni bir aralığına yayılır) yeniler. Çalışma kitabındaki diğer formüller, dinamik dizi formülleri tarafından kullanılsa bile, yinelemeli olarak hesaplanmayacaktır. |
| [RefreshDynamicArrayFormulas](../../aspose.cells/workbook/refreshdynamicarrayformulas/#refreshdynamicarrayformulas_1)(bool, CalculationOptions) | Dinamik dizi formüllerini (mevcut verilere göre komşu hücrelerin yeni bir aralığına yayılır) yeniler. |
| [RemoveDigitalSignature](../../aspose.cells/workbook/removedigitalsignature/)() | Bu elektronik tablodan dijital imzayı kaldırır. |
| [RemoveExternalLinks](../../aspose.cells/workbook/removeexternallinks/)() | (**Obsolete.**) Çalışma kitabındaki tüm dış bağlantıları kaldırır. |
| [RemoveMacro](../../aspose.cells/workbook/removemacro/)() | Bu elektronik tablodan VBA/makroyu kaldırır. |
| [RemovePersonalInformation](../../aspose.cells/workbook/removepersonalinformation/)() | Kişisel bilgileri kaldırır. |
| [RemoveUnusedStyles](../../aspose.cells/workbook/removeunusedstyles/)() | Kullanılmayan tüm stilleri kaldır. |
| [Replace](../../aspose.cells/workbook/replace/#replace)(bool, object) | Hücrelerin değerlerini yeni verilerle değiştirir. |
| [Replace](../../aspose.cells/workbook/replace/#replace_1)(int, object) | Hücrelerin değerlerini yeni verilerle değiştirir. |
| [Replace](../../aspose.cells/workbook/replace/#replace_6)(string, DataTable) | Hücrelerin değerlerini bir DataTable'dan gelen verilerle değiştirir. |
| [Replace](../../aspose.cells/workbook/replace/#replace_2)(string, double) | Bir hücrenin değerini yeni bir double ile değiştirir. |
| [Replace](../../aspose.cells/workbook/replace/#replace_4)(string, int) | Bir hücrenin değerini yeni bir integer ile değiştirir. |
| [Replace](../../aspose.cells/workbook/replace/#replace_7)(string, string) | Bir hücrenin değerini yeni bir string ile değiştirir. |
| [Replace](../../aspose.cells/workbook/replace/#replace_3)(string, double[], bool) | Hücrelerin değerlerini bir double dizisiyle değiştirir. |
| [Replace](../../aspose.cells/workbook/replace/#replace_5)(string, int[], bool) | Hücrelerin değerlerini bir integer dizisiyle değiştirir. |
| [Replace](../../aspose.cells/workbook/replace/#replace_8)(string, string, ReplaceOptions) | Bir hücrenin değerini yeni bir string ile değiştirir. |
| [Replace](../../aspose.cells/workbook/replace/#replace_9)(string, string[], bool) | Bir hücrenin değerini yeni bir string dizisiyle değiştirir. |
| [Save](../../aspose.cells/workbook/save/#save_2)(string) | Çalışma kitabını diske kaydeder. |
| [Save](../../aspose.cells/workbook/save/#save)(Stream, SaveFormat) | Çalışma kitabını akışa kaydeder. |
| [Save](../../aspose.cells/workbook/save/#save_1)(Stream, SaveOptions) | Çalışma kitabını akışa kaydeder. |
| [Save](../../aspose.cells/workbook/save/#save_3)(string, SaveFormat) | Çalışma kitabını diske kaydeder. |
| [Save](../../aspose.cells/workbook/save/#save_4)(string, SaveOptions) | Çalışma kitabını diske kaydeder. |
| [Save](../../aspose.cells/workbook/save/#save_5)(HttpResponse, string, ContentDisposition, SaveOptions) | Sonuç elektronik tablosunu oluşturur ve istemciye aktarır, ardından tarayıcıda veya MS Workbook'ta açar. |
| [Save](../../aspose.cells/workbook/save/#save_6)(HttpResponse, string, ContentDisposition, SaveOptions, bool) | Sonuç elektronik tablosunu oluşturur ve istemciye aktarır, ardından tarayıcıda veya MS Workbook'ta açar. |
| [SaveToStream](../../aspose.cells/workbook/savetostream/)() | Excel dosyasını bir MemoryStream nesnesine Excel97-2003 xls dosyası olarak kaydeder ve döndürür. |
| [SetDigitalSignature](../../aspose.cells/workbook/setdigitalsignature/)(DigitalSignatureCollection) | Bir elektronik tablo dosyasına (Excel2007 ve sonrası) dijital imza ekler. |
| [SetEncryptionOptions](../../aspose.cells/workbook/setencryptionoptions/)(EncryptionType, int) | Şifreleme Seçeneklerini Ayarla. |
| [SetThemeColor](../../aspose.cells/workbook/setthemecolor/)(ThemeColorType, Color) | Tema rengini ayarlar |
| [StartAccessCache](../../aspose.cells/workbook/startaccesscache/)(AccessCacheOptions) | Veriye erişmek için önbellekleri kullanan oturumu başlatır. |
| [Unprotect](../../aspose.cells/workbook/unprotect/)(string) | Bir çalışma kitabının korumasını kaldırır. |
| [UnprotectSharedWorkbook](../../aspose.cells/workbook/unprotectsharedworkbook/)(string) | Paylaşılan bir çalışma kitabının korumasını kaldırır. |
| [UpdateCustomFunctionDefinition](../../aspose.cells/workbook/updatecustomfunctiondefinition/)(CustomFunctionDefinition) | Özel işlevlerin tanımını günceller. |
| [UpdateLinkedDataSource](../../aspose.cells/workbook/updatelinkeddatasource/)(Workbook[]) | Bu çalışma kitabı diğer veri kaynaklarına dış bağlantılar içeriyorsa, Aspose.Cells verilen kaynaklardan en son verileri almaya çalışacaktır. |

### Açıklamalar

Workbook sınıfı bir Excel elektronik tablosunu temsil eder. Her elektronik tablo birden fazla çalışma sayfası içerebilir. Sınıfın temel özelliği yerel excel dosyalarını açmak ve kaydetmektir. Sınıf, diğer Workbook'lerden veri kopyalama, iki Workbook'ü birleştirme, Excel'i PDF'e dönüştürme, Excel'i görüntüye render etme ve Excel elektronik tablosunu koruma gibi gelişmiş özelliklere sahiptir.

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class WorkbookDemo
    {
        public static void WorkbookExample()
        {
            // Yeni bir Workbook örneği oluştur
            Workbook workbook = new Workbook();

            // Varsayılan çalışma sayfasına eriş
            Worksheet worksheet = workbook.Worksheets[0];

            // Çalışma kitabının bazı özelliklerini ayarla
            workbook.FileName = "ExampleWorkbook.xlsx";
            workbook.DefaultStyle.Font.Name = "Tahoma";

            // Yeni bir çalışma sayfası ekle
            int newSheetIndex = workbook.Worksheets.Add();
            Worksheet newWorksheet = workbook.Worksheets[newSheetIndex];
            newWorksheet.Name = "NewSheet";

            // Yeni çalışma sayfasına bazı veriler ekle
            newWorksheet.Cells["A1"].PutValue("Hello, Aspose.Cells!");

            // Bazı belge özelliklerini ayarla
            workbook.BuiltInDocumentProperties["Author"].Value = "John Smith";
            workbook.CustomDocumentProperties.Add("Checked by", "Jane");

            // Çalışma kitabını bir dosyaya kaydedin
            workbook.Save("WorkbookExample.xlsx");

            // Bazı özellikleri göster
            Console.WriteLine("Workbook File Name: " + workbook.FileName);
            Console.WriteLine("Default Font: " + workbook.DefaultStyle.Font.Name);
            Console.WriteLine("Author: " + workbook.BuiltInDocumentProperties["Author"].Value);
            Console.WriteLine("Custom Property 'Checked by': " + workbook.CustomDocumentProperties["Checked by"].Value);

            // Çalışma kitabının lisanslı olup olmadığını kontrol et
            Console.WriteLine("Is Licensed: " + workbook.IsLicensed);

            // Çalışma kitabının dijital olarak imzalı olup olmadığını kontrol et
            Console.WriteLine("Is Digitally Signed: " + workbook.IsDigitallySigned);

            // Çalışma kitabının makrolar içerip içermediğini kontrol et
            Console.WriteLine("Has Macros: " + workbook.HasMacro);

            // Çalışma kitabının izlenen değişiklikleri olup olmadığını kontrol et
            Console.WriteLine("Has Revisions: " + workbook.HasRevisions);

            // Stil havuzundaki stil sayısını kontrol et
            Console.WriteLine("Number of Styles in Pool: " + workbook.CountOfStylesInPool);

            // Tema adını kontrol et
            Console.WriteLine("Theme: " + workbook.Theme);

            // Çalışma kitabının bir şifreyle korumalı olup olmadığını kontrol et
            Console.WriteLine("Is Workbook Protected With Password: " + workbook.IsWorkbookProtectedWithPassword);

            // Çalışma kitabının dış bağlantılar içerip içermediğini kontrol et
            Console.WriteLine("Has External Links: " + (workbook.Worksheets.ExternalLinks.Count > 0));

            // Çalışma kitabını serbest bırak
            workbook.Dispose();
        }
    }
}
```

### Ayrıca Bakınız

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


