---
title: "Arayüz IGridJsService"
second_title: "Aspose.Cells için .NET API Referansı"
description: "Aspose.Cells.GridJs.IGridJsService arayüzü. Kontrolcü eylemlerinde kullanılan temel işlem API'leri arayüzünü temsil eder"
type: docs
url: /tr/net/aspose.cells.gridjs/igridjsservice/
---
## IGridJsService interface

Denetleyici eylemlerinde kullanılan temel işlem API'leri arayüzünü temsil eder.

```csharp
public interface IGridJsService : IDisposable
```

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [AddImage](../../aspose.cells.gridjs/igridjsservice/addimage/#addimage)(string, string, string, byte[]) | Yerel dosyadan resim ekleme işlemini uygular, resim baytlarını doğrudan alır. |
| [AddImage](../../aspose.cells.gridjs/igridjsservice/addimage/#addimage_1)(string, string, string, IFormFileCollection) | Yerel dosyadan resim ekleme işlemini uygular, yüklenen form dosyalarını alır. |
| [AddImageByURL](../../aspose.cells.gridjs/igridjsservice/addimagebyurl/)(string, string, string) | Uzak URL'den resim ekleme işlemini uygular. |
| [CheckInCacheForCollaborative](../../aspose.cells.gridjs/igridjsservice/checkincacheforcollaborative/)(string) | Çalışma kitabı örneğinin bellek önbelleğinde olup olmadığını kontrol eder. Bu yöntem yalnızca İşbirlikçi mod için uygulanır. |
| [ClearAllJsonCache](../../aspose.cells.gridjs/igridjsservice/clearalljsoncache/)() | Tüm JSON önbellek girişlerini (bellek ve disk) temizler. |
| [ClearJsonCacheForUid](../../aspose.cells.gridjs/igridjsservice/clearjsoncacheforuid/)(string) | Belirtilen benzersiz kimliğe ait tüm JSON önbellek girişlerini temizler. Kaynak dosyayı dışarıdan değiştirdikten sonra bunu çağırın, böylece bir sonraki istek JSON'u yeniden oluşturur. |
| [CopyImage](../../aspose.cells.gridjs/igridjsservice/copyimage/)(string, string) | Resim kopyalama işlemini uygular. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid_1)(string, string) | Belirtilen benzersiz kimliğe göre dosya için JSON dizesini alır. |
| [DetailFileJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailfilejsonwithuid/#detailfilejsonwithuid)(Workbook, string, string) | Belirtilen benzersiz kimliğe göre Çalışma Kitabı için JSON dizesini alır. |
| [DetailStreamJson](../../aspose.cells.gridjs/igridjsservice/detailstreamjson/#detailstreamjson_1)(Stream, string) | Çalışma Kitabı için JSON dizesini akıma yazar |
| [DetailStreamJson](../../aspose.cells.gridjs/igridjsservice/detailstreamjson/#detailstreamjson)(Stream, Workbook, string) | Çalışma Kitabı için JSON dizesini akıma yazar |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid_1)(Stream, string, string) | Belirtilen benzersiz kimliğe göre dosya için JSON dizesini akıma yazar. |
| [DetailStreamJsonWithUid](../../aspose.cells.gridjs/igridjsservice/detailstreamjsonwithuid/#detailstreamjsonwithuid)(Stream, Workbook, string, string) | Belirtilen benzersiz kimliğe göre Çalışma Kitabı için JSON dizesini akıma yazar |
| [Download](../../aspose.cells.gridjs/igridjsservice/download/)(string, string, string) | Dosya indirme işlemini uygular |
| [GetFile](../../aspose.cells.gridjs/igridjsservice/getfile/)(string) | Dosya akışını al |
| [GetWarningCallback](../../aspose.cells.gridjs/igridjsservice/getwarningcallback/)() | İçe aktarma dosyası için özel uyarı geri çağrısını alır. |
| [Image](../../aspose.cells.gridjs/igridjsservice/image/)(string, string) | Görselin akışını al. |
| [ImageUrl](../../aspose.cells.gridjs/igridjsservice/imageurl/)(string, string, string) | Görselin URL'sini alır. |
| [LazyLoadingJson](../../aspose.cells.gridjs/igridjsservice/lazyloadingjson/)(string, string) | Belirtilen benzersiz kimliği kullanarak önbellekten dosyadaki belirtilen sayfanın JSON dizesini alır. |
| [LazyLoadingStreamJson](../../aspose.cells.gridjs/igridjsservice/lazyloadingstreamjson/)(Stream, string, string) | Belirtilen benzersiz kimliği kullanarak önbellekten dosyadaki belirtilen sayfanın JSON dizesini akışa yazar.. |
| [Load](../../aspose.cells.gridjs/igridjsservice/load/)(string, string) | Belirtilen benzersiz kimliği kullanarak önbellekten dosyanın JSON dizesini alır, JSON içinde çıktı dosya adını ayarlar. |
| [Ole](../../aspose.cells.gridjs/igridjsservice/ole/)(string, string, int, out string) | Gömülü OLE nesnesinin bayt dizisi verisini alır. |
| [SetWarningCallback](../../aspose.cells.gridjs/igridjsservice/setwarningcallback/)(IWarningCallback) | İçe aktarma dosyası için özel uyarı geri çağrısını ayarlar. |
| [UpdateCell](../../aspose.cells.gridjs/igridjsservice/updatecell/)(string, string) | Güncelleme işlemini uygular. |

### Ayrıca Bakınız

* namespace [Aspose.Cells.GridJs](../../aspose.cells.gridjs/)
* assembly [Aspose.Cells.GridJs](../../)


