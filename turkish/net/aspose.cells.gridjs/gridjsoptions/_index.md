---
title: "Sınıf GridJsOptions"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridJs.GridJsOptions sınıfı. GridJs için tüm yükleme seçeneklerini temsil eder"
type: docs
url: /tr/net/aspose.cells.gridjs/gridjsoptions/
---
## GridJsOptions class

GridJs için tüm yükleme seçeneklerini temsil eder

```csharp
public class GridJsOptions
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [GridJsOptions](gridjsoptions/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [AutoFitColumnsOnLoad](../../aspose.cells.gridjs/gridjsoptions/autofitcolumnsonload/) { get; set; } | Dosya yüklenirken sütun genişliklerinin otomatik ayarlanıp ayarlanmayacağını belirtir, varsayılan değer false'tur. |
| [AutoFitRowsHeightOnLoad](../../aspose.cells.gridjs/gridjsoptions/autofitrowsheightonload/) { get; set; } | Dosya yüklenirken satır yüksekliğinin otomatik ayarlanıp ayarlanmayacağını belirtir, varsayılan değer false'tur. |
| [AutoOptimizeForLargeCells](../../aspose.cells.gridjs/gridjsoptions/autooptimizeforlargecells/) { get; set; } | Büyük hücreli çalışma sayfaları için yükleme performansını otomatik olarak optimize edip etmeyeceğini alır/ayarlar. Yükleme süresini azaltmak için bazı stil /kenarlıkları yok sayar. Varsayılan değer true'tur. |
| [BaseRouteName](../../aspose.cells.gridjs/gridjsoptions/baseroutename/) { get; set; } | GridJs denetleyicisi için yol URL temel adını alır/ayarlar. Varsayılan değer GridJs2'dir. |
| [CustomPdfSaveOptions](../../aspose.cells.gridjs/gridjsoptions/custompdfsaveoptions/) { get; set; } | PDF dışa aktarma için özel PdfSaveOptions'ı alır/ayarlar. Ayarlanırsa, varsayılan seçenekler yerine bu kullanılacaktır. Varsayılan değer null'dır. |
| [EmptySheetMaxCol](../../aspose.cells.gridjs/gridjsoptions/emptysheetmaxcol/) { get; set; } | Boş bir çalışma sayfası için varsayılan maksimum sütunu alır/ayarlar. Varsayılan değer 15'tir. |
| [EmptySheetMaxRow](../../aspose.cells.gridjs/gridjsoptions/emptysheetmaxrow/) { get; set; } | Boş bir çalışma sayfası için varsayılan maksimum satırı alır/ayarlar. Varsayılan değer 12'dir. |
| [EnableChartClientRendering](../../aspose.cells.gridjs/gridjsoptions/enablechartclientrendering/) { get; set; } | İstemci tarafı grafik renderlamasını etkinleştirip etkinleştirmeyeceğini alır/ayarlar. False olarak ayarlanırsa, GridJs yalnızca grafik resimleri/şekilleri üretir ve istemci tarafı grafik renderlaması gerektirmez. Varsayılan değer true'tur. |
| [FileCacheDirectory](../../aspose.cells.gridjs/gridjsoptions/filecachedirectory/) { get; set; } | Alır/Ayarlar elektronik tablo dosyasını depolamak için önbellek dizinini. GridJs'i kullanmadan önce bunu belirli bir yola ayarlamamız gerekir. |
| [FontFolders](../../aspose.cells.gridjs/gridjsoptions/fontfolders/) { get; set; } | Alır/Ayarlar oluşturulan resim/şekillerdeki yazı tipleri için yazı tipi klasörlerini. |
| [IgnoreEmptyContent](../../aspose.cells.gridjs/gridjsoptions/ignoreemptycontent/) { get; set; } | Alır/Ayarlar maksimum aralığın gösterilip gösterilmeyeceğini; bu aralık veri, stil, birleştirilmiş hücreler ve şekilleri içerir. Son satır veya sütun değer ve formül içermeyen ancak özel stil taşıyan hücreler içeriyorsa, bu değer true olduğunda bu satır/sütun gösterilmez. Varsayılan değer true'tur. |
| [IsCollaborative](../../aspose.cells.gridjs/gridjsoptions/iscollaborative/) { get; set; } | Alır/Ayarlar işbirlikli düzenlemeyi destekleyip desteklemeyeceğini, varsayılan false'tur. |
| [IslimitShapeOrImage](../../aspose.cells.gridjs/gridjsoptions/islimitshapeorimage/) { get; set; } | Alır/Ayarlar bir çalışma sayfasındaki toplam görüntülenen şekil/görüntü sayısının sınırlanıp sınırlanmayacağını; true olarak ayarlanırsa, GridJs bir çalışma sayfasındaki görüntülenen şekil veya görüntü sayısını MaxShapeOrImageCount değerine sınırlar. Varsayılan değer true'tur. |
| [IsWasm](../../aspose.cells.gridjs/gridjsoptions/iswasm/) { get; set; } | Alır/Ayarlar GridJs'in bir sunucu süreci yerine tarayıcı WebAssembly ana bilgisayarında çalışıp çalışmayacağını. True olduğunda, FileCacheDirectory / disk / interrupt-thread yolu kullanılmaz ve dosya önbelleği CacheImp'ten gelmelidir, çünkü tarayıcı ana bilgisayarında yerel disk yoktur. Çalışma zamanında kod yolları seçilir, böylece tek bir Aspose.Cells.GridJs.dll her iki ana bilgisayarı da hizmet verir. Varsayılan değer false'tur. |
| [JsonCache](../../aspose.cells.gridjs/gridjsoptions/jsoncache/) { get; set; } | Alır/Ayarlar JSON önbellek yapılandırma seçeneklerini. Oluşturulan çalışma kitabı JSON'ı için hem bellek (L1) hem de disk (L2) önbellek davranışını kontrol eder. |
| [LazyLoading](../../aspose.cells.gridjs/gridjsoptions/lazyloading/) { get; set; } | Alır/Ayarlar yalnızca etkin çalışma sayfasının yüklenip yüklenmeyeceğini, varsayılan false'tur. |
| [MaxPdfSaveSeconds](../../aspose.cells.gridjs/gridjsoptions/maxpdfsaveseconds/) { get; set; } | Alır/Ayarlar PDF'ye kaydedilirken maksimum zaman aşımı saniyesini. Varsayılan değer 10'dur. |
| [MaxShapeOrImageCount](../../aspose.cells.gridjs/gridjsoptions/maxshapeorimagecount/) { get; set; } | Alır/Ayarlar etkin sayfadaki görüntülenen şekil veya görüntülerin toplam sayısını, IslimitShapeOrImage=true olduğunda etkili olur. Varsayılan değer 100'dür. |
| [MaxShapeOrImageWidthOrHeight](../../aspose.cells.gridjs/gridjsoptions/maxshapeorimagewidthorheight/) { get; set; } | Alır/Ayarlar bir şekil veya görüntünün maksimum genişlik veya yüksekliğini, GridJs bu genişlik veya yüksekliği aşan şekil veya görüntüyü yok sayar, IslimitShapeOrImage=true olduğunda etkili olur. Varsayılan değer 10000'dir. |
| [MaxTotalShapeOrImageCount](../../aspose.cells.gridjs/gridjsoptions/maxtotalshapeorimagecount/) { get; set; } | Alır/Ayarlar çalışma kitabındaki görüntülenen şekil veya görüntülerin toplam sayısını, IslimitShapeOrImage=true olduğunda etkili olur. Varsayılan değer 300'dür. |
| [MessageTopic](../../aspose.cells.gridjs/gridjsoptions/messagetopic/) { get; set; } | Alır/Ayarlar "\/topic" ile başlayan websocket hedeflerini. Varsayılan "\/topic\/opr"'dir. Yalnızca işbirlikli modda kullanılır. |
| [PictureCacheDirectory](../../aspose.cells.gridjs/gridjsoptions/picturecachedirectory/) { get; set; } | Alır/Ayarlar resimler için önbellek dizinini. (Bu, GridJsWorkbook.CacheImp null olduğunda etkili olur) Varsayılan yol, FileCacheDirectory içinde "_piccache" olacaktır. |
| [SameImageDetecting](../../aspose.cells.gridjs/gridjsoptions/sameimagedetecting/) { get; set; } | Alır/Ayarlar görüntülerin aynı kaynağa sahip olup olmadığını kontrol edip etmeyeceğini, varsayılan true'tır, varsayılan değer true'tur. |
| [SaveHtmlAsZip](../../aspose.cells.gridjs/gridjsoptions/savehtmlaszip/) { get; set; } | Alır/Ayarlar HTML dosyasının zip arşivi olarak kaydedilip kaydedilmeyeceğini, varsayılan false'tur. |
| [ShowChartSheet](../../aspose.cells.gridjs/gridjsoptions/showchartsheet/) { get; set; } | Alır/Ayarlar grafik çalışma sayfasının gösterilip gösterilmeyeceğini. Varsayılan değer false'tur. |
| [SkipInvisibleShapes](../../aspose.cells.gridjs/gridjsoptions/skipinvisibleshapes/) { get; set; } | Alır/Ayarlar UI'da görünmeyen şekillerin atlanıp atlanmayacağını, varsayılan değer true'tur. |
| [UsePrintArea](../../aspose.cells.gridjs/gridjsoptions/useprintarea/) { get; set; } | Alır/Ayarlar çalışma sayfası PrintArea için PageSetup ayarı içerdiğinde UI görüntüleme aralığı için PageSetup.PrintArea kullanılmasını, varsayılan değer false'tur. |

## Alanlar

| Ad | Açıklama |
| --- | --- |
| [CacheImp](../../aspose.cells.gridjs/gridjsoptions/cacheimp/) | Önbellek depolama için özel uygulama. Önbelleği akış biçiminde depolamak istiyorsanız, bunu ayarlamanız ve uygulamanız gerekir. Bir WebAssembly ana bilgisayarı (IsWasm = true) bunu ayarlamalıdır, çünkü varsayılan dosya önbelleği için yerel disk yoktur. |
| [RedactionUseClientGenerateId](../../aspose.cells.gridjs/gridjsoptions/redactionuseclientgenerateid/) | Kırpma ile ilgili işlemlerde gerçek şekil kimliği yerine istemci tarafından oluşturulan kimliğin kullanılıp kullanılmayacağını gösterir. |

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


