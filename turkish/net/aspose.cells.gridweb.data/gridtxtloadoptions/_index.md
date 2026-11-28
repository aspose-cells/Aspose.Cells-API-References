---
title: "Sınıf GridTxtLoadOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridWeb.Data.GridTxtLoadOptions sınıfı. Metin dosyasını yüklemek için seçenekleri temsil eder"
type: docs
url: /tr/net/aspose.cells.gridweb.data/gridtxtloadoptions/
---
## GridTxtLoadOptions class

Metin dosyası yükleme seçeneklerini temsil eder.

```csharp
[Obsolete("This class will be obsoleted after stand alone dll usage of cells public api,instead you can use Aspose.Cells.TxtLoadOptions ")]
public class GridTxtLoadOptions : GridLoadOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [GridTxtLoadOptions](gridtxtloadoptions/)() | Metin dosyası yükleme seçeneklerini oluşturur. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AutoFilter](../../aspose.cells.gridweb.data/gridloadoptions/autofilter/) { get; set; } | Dosyalar yüklenirken verilerin otomatik filtrelenip filtrelenmeyeceğini gösterir. ([`GridLoadOptions`](../gridloadoptions/) sınıfından devralınmıştır.) |
| [CheckDataValid](../../aspose.cells.gridweb.data/gridloadoptions/checkdatavalid/) { get; set; } | Şablon dosyasındaki verilerin geçerli olup olmadığını kontrol eder. ([`GridLoadOptions`](../gridloadoptions/) sınıfından devralınmıştır.) |
| [CheckExcelRestriction](../../aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/) { get; set; } | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde Excel dosyasının kısıtlamalarının kontrol edilip edilmediği. Örneğin, Excel 32K'dan uzun bir dize değerinin girilmesine izin vermez. Cell.PutValue(string) gibi bir yöntemle 32K'dan uzun bir değer girerseniz ve bu özellik true ise bir İstisna alırsınız. Özellik false ise, girdiğiniz dize değerini hücrenin değeri olarak kabul ederiz, böylece daha sonra CSV gibi diğer dosya formatları için tam dize değerini çıktılayabilirsiniz. Ancak, Excel dosya formatı için geçersiz bir değer ayarladıysanız, çalışma kitabını daha sonra Excel dosya formatı olarak kaydetmemelisiniz. Aksi takdirde oluşturulan Excel dosyasında beklenmeyen hatalar oluşabilir. ([`GridLoadOptions`](../gridloadoptions/) sınıfından devralınmıştır.) |
| [ConvertDateTimeData](../../aspose.cells.gridweb.data/gridtxtloadoptions/convertdatetimedata/) { get; set; } | Metin dosyasındaki dizenin tarih verisine dönüştürülüp dönüştürülmediğini gösteren bir değeri alır veya ayarlar. |
| [ConvertNumericData](../../aspose.cells.gridweb.data/gridtxtloadoptions/convertnumericdata/) { get; set; } | Metin dosyasındaki dizenin sayısal veriye dönüştürülüp dönüştürülmediğini gösteren bir değeri alır veya ayarlar. |
| [Encoding](../../aspose.cells.gridweb.data/gridtxtloadoptions/encoding/) { get; set; } | Varsayılan kodlamayı alır ve ayarlar. Yalnızca csv dosyası için geçerlidir. |
| [ExtendToNextSheet](../../aspose.cells.gridweb.data/gridtxtloadoptions/extendtonextsheet/) { get; set; } | Veri satırları veya sütunları sınırı aştığında verinin bir sonraki sayfaya genişletilip genişletilmeyeceği. Bu özellik true ise, fazla veri mevcut sayfanın arkasındaki bir sonraki sayfaya genişletilir (eğer mevcut sayfa son sayfa ise, yeni sayfa mevcut çalışma kitabına eklenir). Bu özellik false ise, sınırı aşan veri yok sayılır. Varsayılan değer false; |
| [HasFormula](../../aspose.cells.gridweb.data/gridtxtloadoptions/hasformula/) { get; set; } | Metnin "=" ile başlıyorsa formül olup olmadığını gösterir. |
| [HasTextQualifier](../../aspose.cells.gridweb.data/gridtxtloadoptions/hastextqualifier/) { get; set; } | Hücre değeri için metin niteleyicisinin olup olmadığı. Varsayılan değer true'tur. |
| [IgnoreNotPrinted](../../aspose.cells.gridweb.data/gridloadoptions/ignorenotprinted/) { get; set; } | Dosyayı doğrudan yazdırırken basılmayan verileri yok say. ([`GridLoadOptions`](../gridloadoptions/) sınıfından devralınmıştır.) |
| [IsMultiEncoded](../../aspose.cells.gridweb.data/gridtxtloadoptions/ismultiencoded/) { get; set; } | True, dosyanın birden fazla kodlama içerdiği anlamına gelir. |
| [KeepPrecision](../../aspose.cells.gridweb.data/gridtxtloadoptions/keepprecision/) { get; set; } | Uzunluğu 15 ise bir dize değerinin ayrılmayacağını belirtir. |
| [KeepUnparsedData](../../aspose.cells.gridweb.data/gridloadoptions/keepunparseddata/) { get; set; } | Şablon dosyasından yüklendiğinde Çalışma Kitabı için ayrıştırılmamış verilerin bellekte tutulup tutulmayacağı. Varsayılan değer true. ([`GridLoadOptions`](../gridloadoptions/) sınıfından devralınmıştır.) |
| [OnlyAuto](../../aspose.cells.gridweb.data/gridloadoptions/onlyauto/) { get; set; } | Yüksekliği özelleştirilmemiş satırların yalnızca sığdırılıp sığdırılmayacağını gösterir. ([`GridLoadOptions`](../gridloadoptions/) sınıfından devralınmıştır.) |
| [ParsingFormulaOnOpen](../../aspose.cells.gridweb.data/gridloadoptions/parsingformulaonopen/) { get; set; } | Dosya okunurken formülün ayrıştırılıp ayrıştırılmayacağını gösterir. ([`GridLoadOptions`](../gridloadoptions/) sınıfından devralınmıştır.) |
| [ParsingPivotCachedRecords](../../aspose.cells.gridweb.data/gridloadoptions/parsingpivotcachedrecords/) { get; set; } | Dosya yüklenirken pivot önbellek kayıtlarının ayrıştırılıp ayrıştırılmayacağını gösterir. Varsayılan değer false. ([`GridLoadOptions`](../gridloadoptions/) sınıfından devralınmıştır.) |
| [Password](../../aspose.cells.gridweb.data/gridloadoptions/password/) { get; set; } | Çalışma kitabının şifresini alır ve ayarlar. ([`GridLoadOptions`](../gridloadoptions/) sınıfından devralınmıştır.) |
| [PreservePaddingSpacesInFormula](../../aspose.cells.gridweb.data/gridloadoptions/preservepaddingspacesinformula/) { get; set; } | Formüller alınırken ve ayarlanırken formül tokenları arasında eklenen boşluk ve satır sonlarının korunup korunmayacağını gösterir. Varsayılan değer false. ([`GridLoadOptions`](../gridloadoptions/) sınıfından devralınmıştır.) |
| [Separator](../../aspose.cells.gridweb.data/gridtxtloadoptions/separator/) { get; set; } | Metin dosyasının karakter ayırıcıyı alır ve ayarlar. |
| [SeparatorString](../../aspose.cells.gridweb.data/gridtxtloadoptions/separatorstring/) { get; set; } | Ayırıcı olarak bir dize değerini alır ve ayarlar. |
| [TextQualifier](../../aspose.cells.gridweb.data/gridtxtloadoptions/textqualifier/) { get; set; } | Hücre değerleri için metin niteleyicisini belirtir. Varsayılan niteleyici '\"' dir. |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells.gridweb.data/gridtxtloadoptions/treatconsecutivedelimitersasone/) { get; set; } | Ardışık sınırlayıcıların tek olarak ele alınıp alınmayacağı. |
| [TreatQuotePrefixAsValue](../../aspose.cells.gridweb.data/gridtxtloadoptions/treatquoteprefixasvalue/) { get; set; } | Başlangıçtaki tek tırnak işaretinin bir hücrenin değeri içinde bir parça olarak alınması gerekip gerekmediğini gösterir. Varsayılan değer true. False ise, başlangıçtaki tek tırnak ilgili hücrenin değerinden kaldırılır ve hücre için [`QuotePrefix`](../../aspose.cells.gridweb/gridtableitemstyle/quoteprefix/) true olarak ayarlanır. |

### Ayrıca Bakınız

* class [GridLoadOptions](../gridloadoptions/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


