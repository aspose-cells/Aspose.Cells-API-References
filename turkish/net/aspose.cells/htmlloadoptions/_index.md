---
title: "Class HtmlLoadOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.HtmlLoadOptions sınıfı. HTML dosyası içe aktarılırken seçenekleri temsil eder."
type: docs
url: /tr/net/aspose.cells/htmlloadoptions/
---
## HtmlLoadOptions class

HTML dosyası içe aktarılırken seçenekleri temsil eder.

```csharp
public class HtmlLoadOptions : AbstractTextLoadOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [HtmlLoadOptions](htmlloadoptions/#constructor)() | Dosyayı yükleme seçeneklerini oluşturur. |
| [HtmlLoadOptions](htmlloadoptions/#constructor_1)(LoadFormat) | Dosyayı yükleme seçeneklerini oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AttachedFilesDirectory](../../aspose.cells/htmlloadoptions/attachedfilesdirectory/) { get; set; } | (**Obsolete.**) Ekli dosyaların kaydedileceği dizin. |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter/) { get; set; } | Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmeyeceğini gösterir.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [AutoFitColsAndRows](../../aspose.cells/htmlloadoptions/autofitcolsandrows/) { get; set; } | Sütun ve satırların otomatik sığdırılıp sığdırılmayacağını gösterir. Varsayılan değer false'tur. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions/) { get; set; } | Otomatik sığdırma seçeneklerini alır ve ayarlar(Inherited from [`LoadOptions`](../loadoptions/).) |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid/) { get; set; } | Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol eder.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction/) { get; set; } | Kullanıcı hücreyle ilgili nesneleri değiştirdiğinde excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi 32K'dan uzun bir değer girdiğinizde, bu özellik true ise bir Exception alırsınız. Bu özellik false ise, girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak, excel dosya formatı için geçersiz bir değer ayarladıysanız, çalışma kitabını daha sonra excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan excel dosyasında beklenmeyen hatalar oluşabilir.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata/) { get; set; } | Metin dosyasındaki dizeyin tarih verisine dönüştürülüp dönüştürülmediğini gösteren bir değeri alır veya ayarlar. Varsayılan değer true'tir.(Inherited from [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [ConvertFormulasData](../../aspose.cells/htmlloadoptions/convertformulasdata/) { get; set; } | (**Obsolete.**) true ise, dize değeri '=' karakteriyle başladığında dizeyi formüle dönüştür, varsayılan değer false'tur. |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata/) { get; set; } | Metin dosyasındaki dizeyin sayısal veriye dönüştürülüp dönüştürülmediğini gösteren bir değeri alır veya ayarlar. Varsayılan değer true'tir.(Inherited from [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo/) { get; set; } | Yüklenmek üzere olan Workbook için kullanılan bölgesel ayarları alır veya ayarlar.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings/) { get; } | workbook için stil başlatma varsayılan ayarlarını alır(Inherited from [`LoadOptions`](../loadoptions/).) |
| [DeleteRedundantSpaces](../../aspose.cells/htmlloadoptions/deleteredundantspaces/) { get; set; } | Metin satırları `<br>` etiketiyle sarıldığında gereksiz boşlukların silinip silinmeyeceğini gösterir. Varsayılan değer false'dur. |
| [DetectLaTeX](../../aspose.cells/htmlloadoptions/detectlatex/) { get; set; } | HTML dosyasında LaTeX formülünün algılanıp algılanmayacağını gösterir. Varsayılan değer false'dur. |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding/) { get; set; } | Varsayılan kodlamayı alır ve ayarlar. Yalnızca csv dosyası için geçerlidir. (Kalıtım alınan [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs/) { get; set; } | Bireysel font yapılandırmalarını alır ve ayarlar. Bu [`LoadOptions`](../loadoptions/) ile yüklenen [`Workbook`](../workbook/) için yalnızca çalışır.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [HasFormula](../../aspose.cells/htmlloadoptions/hasformula/) { get; set; } | Metnin "=" ile başlıyorsa formül olup olmadığını gösterir. |
| [HyperlinkLoadMode](../../aspose.cells/htmlloadoptions/hyperlinkloadmode/) { get; set; } | HTML yüklenirken köprülerin nasıl yükleneceğini belirtir. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted/) { get; set; } | Dosyayı doğrudan yazdırırken basılmayan verileri yoksayar(Inherited from [`LoadOptions`](../loadoptions/).) |
| [IgnoreUselessShapes](../../aspose.cells/loadoptions/ignoreuselessshapes/) { get; set; } | Kullanışsız şekillerin yoksayılıp yoksayılmayacağını gösterir.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor/) { get; set; } | Kesinti izleyicisini alır ve ayarlar.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision/) { get; set; } | Uzunluğu 15 ise bir dize değerinin ayrılıp ayrılmayacağını gösterir. (Kalıtım alınan [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata/) { get; set; } | Şablon dosyasından yüklendiğinde Workbook için ayrıştırılmamış verilerin bellekte tutulup tutulmayacağını belirtir. Varsayılan true'tur.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode/) { get; set; } | Dosyayı kaydeden CountryCode'a dayalı olarak Workbook sürümünün kullanıcı arayüzü dilini alır veya ayarlar.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler/) { get; set; } | Şablon dosyası okunurken hücre verilerini işlemek için veri işleyicisi.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter/) { get; set; } | Verilerin nasıl yükleneceğini belirten filtre.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat/) { get; } | Yükleme biçimini alır.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [LoadFormulas](../../aspose.cells/htmlloadoptions/loadformulas/) { get; set; } | Orijinal html dosyası formüller içeriyorsa formüllerin içe aktarılıp aktarılmayacağını gösterir. |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy/) { get; set; } | Dize değerini sayıya veya tarih‑zamanına dönüştürürken ayrıştırılan değerlere stil uygulama stratejisini gösterir. (Kalıtım alınan [`AbstractTextLoadOptions`](../abstracttextloadoptions/).) |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting/) { get; set; } | Yüklenen workbook için bellek modunu alır veya ayarlar(Inherited from [`LoadOptions`](../loadoptions/).) |
| [ParagrahLayoutMode](../../aspose.cells/htmlloadoptions/paragrahlayoutmode/) { get; set; } | (**Obsolete.**) HTML yüklenirken HTML &lt;p&gt; öğelerinin nasıl işleneceğini belirtir. Varsayılan değer Normal'dir. |
| [ParagraphLayoutMode](../../aspose.cells/htmlloadoptions/paragraphlayoutmode/) { get; set; } | HTML yüklenirken HTML &lt;p&gt; öğelerinin nasıl işleneceğini belirtir. Varsayılan değer Normal'dir. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen/) { get; set; } | Dosya okunurken formülün ayrıştırılıp ayrıştırılmayacağını gösterir.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords/) { get; set; } | Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmayacağını gösterir. Varsayılan değer false'tur.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [Password](../../aspose.cells/loadoptions/password/) { get; set; } | Workbook'un şifresini alır ve ayarlar.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells/loadoptions/preservepaddingspacesinformula/) { get; set; } | Formülleri alırken ve ayarlarken formül belirteçleri arasına eklenen boşlukları ve satır sonlarını koruyup korumayacağını gösterir. Varsayılan değer false'tur. (Miras alınan [`LoadOptions`](../loadoptions/).) |
| [ProgId](../../aspose.cells/htmlloadoptions/progid/) { get; } | Dosyanın oluşturulması için program kimliğini alır. Yalnızca MHT dosyaları için. |
| [Region](../../aspose.cells/loadoptions/region/) { get; set; } | Yüklenmek üzere olan Workbook için kullanılan bölgesel ayarları alır veya ayarlar.(Inherited from [`LoadOptions`](../loadoptions/).) |
| [StandardFont](../../aspose.cells/loadoptions/standardfont/) { get; set; } | (**Obsolete.**) Varsayılan standart yazı tipi adını ayarlar(Miras alınan [`LoadOptions`](../loadoptions/).) |
| [StandardFontSize](../../aspose.cells/loadoptions/standardfontsize/) { get; set; } | (**Obsolete.**) Varsayılan standart yazı tipi boyutunu ayarlar. (Miras alınan [`LoadOptions`](../loadoptions/).) |
| [StreamProvider](../../aspose.cells/htmlloadoptions/streamprovider/) { get; set; } | Nesneleri içe aktarmak için StreamProviderImportHtmlFile'ı alır veya ayarlar. |
| [SupportDivTag](../../aspose.cells/htmlloadoptions/supportdivtag/) { get; set; } | HTML dosyası `<div>` etiketini içerdiğinde düzenin desteklenip desteklenmeyeceğini gösterir. Varsayılan değer false'dur. |
| [TableLoadOptions](../../aspose.cells/htmlloadoptions/tableloadoptions/) { get; } | HtmlTableLoadOptionCollection örneğini al |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback/) { get; set; } | Uyarı geri çağrısını alır veya ayarlar. (Miras alınan [`LoadOptions`](../loadoptions/).) |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize/)(PaperSizeType) | Varsayılan yazıcının ayarlarından varsayılan baskı kağıdı boyutunu ayarlar. (Miras alınan [`LoadOptions`](../loadoptions/).) |

### Örnekler

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.IO;

    public class HtmlLoadOptionsDemo
    {
        public static void HtmlLoadOptionsExample()
        {
            // HtmlLoadOptions bir örnek oluştur.
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            loadOptions.LoadFormulas = true;
            loadOptions.SupportDivTag = true;
            loadOptions.DeleteRedundantSpaces = true;
            loadOptions.AutoFitColsAndRows = true;
            loadOptions.HasFormula = true;
            loadOptions.Encoding = System.Text.Encoding.UTF8;
            loadOptions.LoadStyleStrategy = TxtLoadStyleStrategy.None;
            loadOptions.ConvertNumericData = true;
            loadOptions.ConvertDateTimeData = true;
            loadOptions.KeepPrecision = true;
            loadOptions.ParsingFormulaOnOpen = true;
            loadOptions.ParsingPivotCachedRecords = true;
            loadOptions.IgnoreNotPrinted = true;
            loadOptions.CheckDataValid = true;
            loadOptions.CheckExcelRestriction = true;
            loadOptions.KeepUnparsedData = true;
            loadOptions.AutoFilter = true;
            loadOptions.IgnoreUselessShapes = true;
            loadOptions.PreservePaddingSpacesInFormula = true;

            // HtmlLoadOptions kullanarak bir HTML dosyasını Workbook içine yükle.
            Workbook workbook = new Workbook("HtmlLoadOptionsExample_original.html", loadOptions);

            // Çalışma kitabını bir Excel dosyasına kaydet
            workbook.Save("HtmlLoadOptionsExample.xlsx");

            return;
        }
    }
}
```

### Ayrıca Bakınız

* class [AbstractTextLoadOptions](../abstracttextloadoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


