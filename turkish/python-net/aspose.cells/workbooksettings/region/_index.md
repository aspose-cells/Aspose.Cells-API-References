---
title: region mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 520
url: /tr/python-net/aspose.cells/workbooksettings/region/
is_root: false
---
##  region mülk

Çalışma kitabı için bölgesel ayarları alır veya ayarlar.

###  Notlar

1. Şablon dosyasından yüklenen bir çalışma kitabı için Aspose.Cells bileşeni tarafından kullanılan bölgesel ayarlar:
Ben). Bir XLS dosyası için, bölgesel ayarlar için tanımlanmış alanlar vardır ve MS Excel, XLS dosyasını kaydederken bölgesel ayarlar verilerini dosyaya kaydeder.
Bu nedenle, çalışma kitabı için şablon dosyasında kaydedilen region'i kullanıyoruz.
XLS dosyasında kayıtlı region'i kullanmak istemiyorsanız, lütfen şablon dosyasını yükledikten sonra onu beklenen değere (CountryCode.Default gibi) sıfırlayın.
Ve XLS dosyasını kaydederken kullanıcı tarafından belirtilen değeri (bu yöntemle) dosyaya da kaydederiz.
ii). XLSX, XLSB...vb. gibi diğer dosya formatları için, dosya formatı belirtiminde bölgesel ayarlar için tanımlanmış bir alan yoktur.
Bu nedenle, çalışma kitabı için uygulama ortamının bölgesel ayarlarını kullanıyoruz.
Ve kullanıcı tarafından belirlenen değer (bu yöntemle), bu dosya biçimleriyle oluşturulan dosyalar için tutulamaz.
2. MS Excel'deki görünüm efekti için:
Burada uygulanan bölgesel ayarlar, oluşturulan dosyayı MS Excel ile görüntülerken değil, yalnızca Aspose.Cells bileşeni ile çalışma zamanında etkili olabilir.
MS Excel ile görüntülerken/düzenlerken, belirtilen bölgesel ayarlar verilerinin kaydedildiği oluşturulan XLS dosyası için bile,
MS Excel tarafından biçimlendirme yapmak için kullanılan region, her zaman MS Excel'in çalıştığı ortamın varsayılan bölgesel ayarlarıdır,
dosyaya kaydedilen değil. MS Excel'in davranışıdır ve kodla değiştirilemez.
###  Tanım:
```python
@property
def region(self):
    ...
@region.setter
def region(self, value):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [CountryCode](/cells/tr/python-net/aspose.cells/countrycode)
* sınıf [WorkbookSettings](/cells/tr/python-net/aspose.cells/workbooksettings)
