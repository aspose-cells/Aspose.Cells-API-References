---
title: LoadFilter sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 1010
url: /tr/python-net/aspose.cells/loadfilter/
is_root: false
---
##  LoadFilter sınıfı
Çalışma kitabını şablondan yüklerken veri yüklemek için seçenekler sağlayan filtreyi temsil eder.



LoadFilter türü aşağıdaki üyeleri gösterir:

###  İnşaatçılar
| Yapıcı| Tanım|
| :- | :- |
| [LoadFilter()](/cells/tr/python-net/aspose.cells/loadfilter/__init__/#) | LoadDataFilterOptions.All varsayılan filtre seçenekleriyle bir LoadFilter oluşturur.|
| [LoadFilter(opts)](/cells/tr/python-net/aspose.cells/loadfilter/__init__/#LoadDataFilterOptions) | Verilen filtre seçenekleriyle bir LoadFilter oluşturur.|


###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [load_data_filter_options](/cells/tr/python-net/aspose.cells/loadfilter/load_data_filter_options) | Hangi verilerin yüklenmesi gerektiğini gösteren filtre seçenekleri.|
| [sheets_in_loading_order](/cells/tr/python-net/aspose.cells/loadfilter/sheets_in_loading_order) | Sayfaları (endeksleri) ve yüklenecek sırayı belirtir.<br/>Varsayılan, boştur, bu da şablon dosyasındaki tüm sayfaların varsayılan sırayla yüklenmesini belirtir.<br/> Null değilse ve bazı sayfaların dizini döndürülen dizide değilse, sayfa yüklenmeyecektir.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [start_sheet(sheet)](/cells/tr/python-net/aspose.cells/loadfilter/start_sheet/#Worksheet) | Belirli bir çalışma sayfasını yüklemeden önce filtre seçeneklerini hazırlar.<br/>Kullanıcının LoadFilter uygulaması, LoadDataFilterOptions'ı burada değiştirebilir<br/> Bu çalışma sayfası için verilerin nasıl yükleneceğini belirtmek için.|



###  Notlar

Kullanıcı, verilerin nasıl yükleneceğini belirtmek için filtre seçeneklerini belirleyebilir veya kendi LoadFilter'ini uygulayabilir.

###  Ayrıca bakınız
* modül [aspose.cells](..)
