---
title: "Sınıf Config"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridJs.Config sınıfı. GridJs için tüm statik ayarları temsil eder."
type: docs
url: /tr/net/aspose.cells.gridjs/config/
---
## Config class

GridJs için tüm statik ayarları temsil eder

```csharp
public class Config
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [Config](config/)() | Varsayılan yapıcı. |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| static [AutoFitColumnsOnLoad](../../aspose.cells.gridjs/config/autofitcolumnsonload/) { get; set; } | Dosya yüklenirken sütun genişliklerinin otomatik ayarlanıp ayarlanmayacağını belirtir. Varsayılan değer `false`'dur. Uyarı: Bunu `true` olarak ayarlamak, yükleme sonrasında tüm sütunların otomatik ayarlanmasını gerçekleştirir ve bu, performans üzerinde belirgin bir etki yaratabilir. |
| static [AutoFitRowsHeightOnLoad](../../aspose.cells.gridjs/config/autofitrowsheightonload/) { get; set; } | Dosya yüklenirken satır yüksekliklerinin otomatik ayarlanıp ayarlanmayacağını belirtir. Varsayılan değer `false`'dur. Uyarı: Bunu `true` olarak ayarlamak, yükleme sonrasında tüm satırların otomatik ayarlanmasını gerçekleştirir ve bu, performans üzerinde belirgin bir etki yaratabilir. |
| static [AutoOptimizeForLargeCells](../../aspose.cells.gridjs/config/autooptimizeforlargecells/) { get; set; } | Büyük hücreli çalışma sayfaları için yükleme performansını otomatik olarak optimize edip etmeyeceğini alır/ayarlar. Yükleme süresini azaltmak için bazı stil /kenarlıkları yok sayar. Varsayılan değer true'tur. |
| static [BaseRouteName](../../aspose.cells.gridjs/config/baseroutename/) { get; set; } | GridJs denetleyici URL'si için temel yol adını alır/ayarlar. Varsayılan "/GridJs2"'dir. |
| static [CustomPdfSaveOptions](../../aspose.cells.gridjs/config/custompdfsaveoptions/) { get; set; } | PDF dışa aktarma için özel PdfSaveOptions'ı alır/ayarlar. Ayarlanırsa, varsayılan seçenekler yerine bu kullanılacaktır. Varsayılan değer null'dır. |
| static [EmptySheetMaxCol](../../aspose.cells.gridjs/config/emptysheetmaxcol/) { get; set; } | Boş bir çalışma sayfası için varsayılan maksimum sütunu alır/ayarlar. Varsayılan değer 15'tir. |
| static [EmptySheetMaxRow](../../aspose.cells.gridjs/config/emptysheetmaxrow/) { get; set; } | Boş bir çalışma sayfası için varsayılan maksimum satırı alır/ayarlar. Varsayılan değer 12'dir. |
| static [EnableChartClientRendering](../../aspose.cells.gridjs/config/enablechartclientrendering/) { get; set; } | İstemci tarafı grafik render'ını etkinleştirip etkinleştirmeyeceğini alır/ayarlar. false olarak ayarlanırsa, GridJs yalnızca sunucu tarafından oluşturulan grafik görüntüleri/şekilleri kullanır. Varsayılan değer true'tir. |
| static [FileCacheDirectory](../../aspose.cells.gridjs/config/filecachedirectory/) { get; set; } | Alır/Ayarlar elektronik tablo dosyasını depolamak için önbellek dizinini. GridJs'i kullanmadan önce bunu belirli bir yola ayarlamamız gerekir. |
| static [IgnoreEmptyContent](../../aspose.cells.gridjs/config/ignoreemptycontent/) { get; set; } | Alır/Ayarlar maksimum aralığın gösterilip gösterilmeyeceğini; bu aralık veri, stil, birleştirilmiş hücreler ve şekilleri içerir. Son satır veya sütun değer ve formül içermeyen ancak özel stil taşıyan hücreler içeriyorsa, bu değer true olduğunda bu satır/sütun gösterilmez. Varsayılan değer true'tur. |
| static [IsCollaborative](../../aspose.cells.gridjs/config/iscollaborative/) { get; set; } | Alır/Ayarlar işbirlikli düzenlemeyi destekleyip desteklemeyeceğini, varsayılan false'tur. |
| static [IslimitShapeOrImage](../../aspose.cells.gridjs/config/islimitshapeorimage/) { get; set; } | Alır/Ayarlar bir çalışma sayfasındaki toplam görüntülenen şekil/görüntü sayısının sınırlanıp sınırlanmayacağını; true olarak ayarlanırsa, GridJs bir çalışma sayfasındaki görüntülenen şekil veya görüntü sayısını MaxShapeOrImageCount değerine sınırlar. Varsayılan değer true'tur. |
| static [IsWasm](../../aspose.cells.gridjs/config/iswasm/) { get; set; } | GridJs'in bir sunucu süreci yerine tarayıcı WebAssembly hostu içinde çalışıp çalışmayacağını alır/ayarlar. true olduğunda, FileCacheDirectory / disk / interrupt-thread yolu kullanılmaz ve dosya önbelleği GridJsOptions.CacheImp üzerinden gelmelidir. GridJsOptions.IsWasm, GridJs hizmeti oluşturulduğunda bunu ayarlar, böylece tek bir Aspose.Cells.GridJs.dll her iki hostu da hizmet verir. Varsayılan değer false'tur. |
| static [JsonCache](../../aspose.cells.gridjs/config/jsoncache/) { get; set; } | Alır/Ayarlar JSON önbellek yapılandırma seçeneklerini. Oluşturulan çalışma kitabı JSON'ı için hem bellek (L1) hem de disk (L2) önbellek davranışını kontrol eder. |
| static [LazyLoading](../../aspose.cells.gridjs/config/lazyloading/) { get; set; } | Alır/Ayarlar yalnızca etkin çalışma sayfasının yüklenip yüklenmeyeceğini, varsayılan false'tur. |
| static [MaxPdfSaveSeconds](../../aspose.cells.gridjs/config/maxpdfsaveseconds/) { get; set; } | Alır/Ayarlar PDF'ye kaydedilirken maksimum zaman aşımı saniyesini. Varsayılan değer 10'dur. |
| static [MaxShapeOrImageCount](../../aspose.cells.gridjs/config/maxshapeorimagecount/) { get; set; } | Alır/Ayarlar etkin sayfadaki görüntülenen şekil veya görüntülerin toplam sayısını, IslimitShapeOrImage=true olduğunda etkili olur. Varsayılan değer 100'dür. |
| static [MaxShapeOrImageWidthOrHeight](../../aspose.cells.gridjs/config/maxshapeorimagewidthorheight/) { get; set; } | Alır/Ayarlar bir şekil veya görüntünün maksimum genişlik veya yüksekliğini, GridJs bu genişlik veya yüksekliği aşan şekil veya görüntüyü yok sayar, IslimitShapeOrImage=true olduğunda etkili olur. Varsayılan değer 10000'dir. |
| static [MaxTotalShapeOrImageCount](../../aspose.cells.gridjs/config/maxtotalshapeorimagecount/) { get; set; } | Alır/Ayarlar çalışma kitabındaki görüntülenen şekil veya görüntülerin toplam sayısını, IslimitShapeOrImage=true olduğunda etkili olur. Varsayılan değer 300'dür. |
| static [MessageTopic](../../aspose.cells.gridjs/config/messagetopic/) { get; set; } | Alır/Ayarlar "\/topic" ile başlayan websocket hedeflerini. Varsayılan "\/topic\/opr"'dir. Yalnızca işbirlikli modda kullanılır. |
| static [PictureCacheDirectory](../../aspose.cells.gridjs/config/picturecachedirectory/) { get; set; } | Alır/Ayarlar resimler için önbellek dizinini. (Bu, GridJsWorkbook.CacheImp null olduğunda etkili olur) Varsayılan yol, FileCacheDirectory içinde "_piccache" olacaktır. |
| static [SameImageDetecting](../../aspose.cells.gridjs/config/sameimagedetecting/) { get; set; } | Alır/Ayarlar görüntülerin aynı kaynağa sahip olup olmadığını kontrol edip etmeyeceğini, varsayılan true'tır, varsayılan değer true'tur. |
| static [SaveHtmlAsZip](../../aspose.cells.gridjs/config/savehtmlaszip/) { get; set; } | Alır/Ayarlar HTML dosyasının zip arşivi olarak kaydedilip kaydedilmeyeceğini, varsayılan false'tur. |
| static [ShowChartSheet](../../aspose.cells.gridjs/config/showchartsheet/) { get; set; } | Alır/Ayarlar grafik çalışma sayfasının gösterilip gösterilmeyeceğini. Varsayılan değer false'tur. |
| static [SkipInvisibleShapes](../../aspose.cells.gridjs/config/skipinvisibleshapes/) { get; set; } | Alır/Ayarlar UI'da görünmeyen şekillerin atlanıp atlanmayacağını, varsayılan değer true'tur. |
| static [UsePrintArea](../../aspose.cells.gridjs/config/useprintarea/) { get; set; } | Alır/Ayarlar çalışma sayfası PrintArea için PageSetup ayarı içerdiğinde UI görüntüleme aralığı için PageSetup.PrintArea kullanılmasını, varsayılan değer false'tur. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| static [SetFontFolder](../../aspose.cells.gridjs/config/setfontfolder/)(string, bool) | Yazı tipleri klasörünü ayarlar |
| static [SetFontFolders](../../aspose.cells.gridjs/config/setfontfolders/)(string[], bool) | Yazı tipi klasörlerini ayarlar |

## Alanlar

| Ad | Açıklama |
| --- | --- |
| static [RedactionUseClientGenerateId](../../aspose.cells.gridjs/config/redactionuseclientgenerateid/) | Kırpma ile ilgili işlemlerde gerçek şekil kimliği yerine istemci tarafından oluşturulan kimliğin kullanılıp kullanılmayacağını gösterir. |

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


