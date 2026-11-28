---
title: "Class GridJsService"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridJs.GridJsService sınıfı. Kontrolcü eylemlerinde kullanılan temel işlem API'lerini sağlar"
type: docs
url: /tr/net/aspose.cells.gridjs/gridjsservice/
---
## GridJsService class

Denetleyici eylemlerinde kullanılan temel işlem API'lerini sağlar.

```csharp
public class GridJsService : IGridJsService
```

## Yapıcılar

| Ad | Açıklama |
| --- | --- |
| [GridJsService](gridjsservice/#constructor)(GridJsOptions) | GridJsService için, seçenek nesnesini kendileri oluşturan ana bilgisayarlar (tarayıcı WASM ana bilgisayarı ve DI olmayan sunucu kurulumları) için yapıcı. |
| [GridJsService](gridjsservice/#constructor_1)(IOptions&lt;GridJsOptions&gt;) | GridJsService için varsayılan yapıcı |

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Settings](../../aspose.cells.gridjs/gridjsservice/settings/) { get; set; } | Çalışma kitabı ayarlarını temsil eder. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [AddImage](../../aspose.cells.gridjs/gridjsservice/addimage/#addimage)(string, string, string, byte[]) | Yerel dosyadan resim ekleme işlemini uygular (dosya baytları JS FormData'dan veya herhangi bir ana bilgisayardan gelir). |
| [AddImage](../../aspose.cells.gridjs/gridjsservice/addimage/#addimage_1)(string, string, string, IFormFileCollection) | Yerel dosyadan resim ekleme işlemini uygular. |
| [AddImageByURL](../../aspose.cells.gridjs/gridjsservice/addimagebyurl/)(string, string, string) | Uzak URL'den resim ekleme işlemini uygular. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/gridjsservice/checkincacheforcollaborative/)(string) | Çalışma kitabı örneğinin bellek önbelleğinde olup olmadığını kontrol eder. Bu yöntem yalnızca İşbirlikçi mod için uygulanır. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/gridjsservice/clearalljsoncache/)() | Tüm JSON önbellek girişlerini (bellek ve disk) temizler. |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/gridjsservice/clearjsoncacheforuid/)(string) | Belirtilen benzersiz kimliğe ait tüm JSON önbellek girişlerini temizler. Kaynak dosyayı dışarıdan değiştirdikten sonra bunu çağırın, böylece bir sonraki istek JSON'u yeniden oluşturur. |
| [CopyImage](../../aspose.cells.gridjs/gridjsservice/copyimage/)(string, string) | Resim kopyalama işlemini uygular. |
| [Destroy](../../aspose.cells.gridjs/gridjsservice/destroy/)() | Bu yöntem yalnızca Java içindir, DisposableBean içinde destroy metodunu uygular, bu metod istek tamamlandığında Spring tarafından otomatik olarak çağrılır, aslında Dispose metodunu çağırır. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid_1)(string, string) | Belirtilen benzersiz kimliğe göre dosya için JSON dizesini alır. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid)(Workbook, string, string) | Belirtilen benzersiz kimliğe göre Çalışma Kitabı için JSON dizesini alır. |
| [DetailStreamJson](../../aspose.cells.gridjs/gridjsservice/detailstreamjson/#detailstreamjson_1)(Stream, string) | Dosya için JSON dizesini akıma yazar. |
| [DetailStreamJson](../../aspose.cells.gridjs/gridjsservice/detailstreamjson/#detailstreamjson)(Stream, Workbook, string) | Çalışma Kitabı için JSON dizesini akıma yazar |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid_1)(Stream, string, string) | Belirtilen benzersiz kimliğe göre dosya için JSON dizesini akıma yazar. |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/gridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid)(Stream, Workbook, string, string) | Belirtilen benzersiz kimliğe göre Çalışma Kitabı için JSON dizesini akıma yazar |
| [Dispose](../../aspose.cells.gridjs/gridjsservice/dispose/)() | Yönetilmeyen kaynakların serbest bırakılması, salınması veya sıfırlanmasıyla ilgili uygulama tanımlı görevleri yürütür. |
| [Download](../../aspose.cells.gridjs/gridjsservice/download/)(string, string, string) | Dosya indirme işlemini uygular |
| [GetFile](../../aspose.cells.gridjs/gridjsservice/getfile/)(string) | Dosya akışını al |
| [GetWarningCallback](../../aspose.cells.gridjs/gridjsservice/getwarningcallback/)() | İçe aktarma dosyası için özel uyarı geri çağrısını alır. |
| [Image](../../aspose.cells.gridjs/gridjsservice/image/)(string, string) | Görselin akışını al. |
| [ImageUrl](../../aspose.cells.gridjs/gridjsservice/imageurl/)(string, string, string) | Görselin URL'sini alır. |
| [LazyLoadingJson](../../aspose.cells.gridjs/gridjsservice/lazyloadingjson/)(string, string) | Belirtilen benzersiz kimliği kullanarak önbellekten dosyadaki belirtilen sayfanın JSON dizesini alır. |
| [LazyLoadingStreamJson](../../aspose.cells.gridjs/gridjsservice/lazyloadingstreamjson/)(Stream, string, string) | Belirtilen benzersiz kimliği kullanarak önbellekten dosyadaki belirtilen sayfanın JSON dizesini akışa yazar.. |
| [Load](../../aspose.cells.gridjs/gridjsservice/load/)(string, string) | Belirtilen benzersiz kimliği kullanarak önbellekten dosyanın JSON dizesini alır, JSON içinde çıktı dosya adını ayarlar. |
| [Ole](../../aspose.cells.gridjs/gridjsservice/ole/)(string, string, int, out string) | Gömülü OLE nesnesinin bayt dizisi verisini alır. |
| [SetWarningCallback](../../aspose.cells.gridjs/gridjsservice/setwarningcallback/)(IWarningCallback) | İçe aktarma dosyası için özel uyarı geri çağrısını ayarlar. |
| [TranslateSheetAsync](../../aspose.cells.gridjs/gridjsservice/translatesheetasync/)(string, string, ITextTranslator, string) | Çalışma sayfasındaki tüm dize değerlerini hedef dile çevir. |
| [UpdateCell](../../aspose.cells.gridjs/gridjsservice/updatecell/)(string, string) | Güncelleme işlemini uygular. |

### Ayrıca Bakınız

* interface [IGridJsService](../igridjsservice/)
* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


