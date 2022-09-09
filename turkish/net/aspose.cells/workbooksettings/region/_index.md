---
title: Region
second_title: Aspose.Cells for .NET API Referansı
description: Çalışma kitabı için bölgesel ayarları alır veya ayarlar.
type: docs
weight: 370
url: /tr/net/aspose.cells/workbooksettings/region/
---
## WorkbookSettings.Region property

Çalışma kitabı için bölgesel ayarları alır veya ayarlar.

```csharp
public CountryCode Region { get; set; }
```

### Notlar

1. Şablon dosyasından yüklenen bir çalışma kitabı için Aspose.Cells bileşeni tarafından kullanılan bölgesel ayarlar: i). Bir XLS dosyası için, bölgesel ayarlar için tanımlanmış alanlar vardır ve MS Excel, XLS dosyasını kaydederken bölgesel ayar verilerini dosyaya kaydeder. Bu nedenle, çalışma kitabı için şablon dosyasında kaydedilen bölgeyi kullanırız. Bunu yapmazsanız XLS dosyasına kaydedilen bölgeyi kullanmak istiyorsanız, lütfen şablon dosyasını yükledikten sonra onu beklenen bölgeye (CountryCode.Default gibi) sıfırlayın. Ve, kullanıcı tarafından belirtilen değeri (bu yöntemle) dosyaya da kaydediyoruz. bir XLS dosyasını kaydederken. ii). XLSX, XLSB...vb. gibi diğer dosya biçimleri için, dosya biçimi belirtiminde bölgesel ayarlar için tanımlanmış bir alan yoktur. Bu nedenle, çalışma kitabı için uygulama ortamının bölgesel ayarlarını kullanırız. Ve, bu dosya formatları ile oluşturulan dosyalar için kullanıcı tarafından belirlenen değer (bu yöntemle) tutulamaz. 2. MS Excel'de görünüm efekti için: Burada uygulanan bölgesel ayarlar yalnızca Aspose.Cells bileşeni ile çalışma zamanında geçerli olabilir, değil oluşturulan dosyayı MS Excel ile görüntülerken. Belirtilen bölgesel ayar verilerinin kaydedildiği oluşturulan XLS dosyası için bile, MS Excel ile görüntülerken/düzenlerken, MS Excel ile biçimlendirme gerçekleştirmek için kullanılan bölge her zaman varsayılandır MS Excel'in çalıştığı ortamın bölgesel ayarları, dosyaya kaydedilen ayar değil. Bu, MS Excel'in davranışıdır ve kodla değiştirilemez.

### Ayrıca bakınız

* enum [CountryCode](../../countrycode)
* class [WorkbookSettings](../../workbooksettings)
* ad alanı [Aspose.Cells](../../workbooksettings)
* toplantı [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->