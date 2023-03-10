---
title: LoadOptions sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 1020
url: /tr/python-net/aspose.cells/loadoptions/
is_root: false
---
##  LoadOptions sınıfı
Dosya yükleme seçeneklerini temsil eder.



LoadOptions türü aşağıdaki üyeleri gösterir:

###  İnşaatçılar
| Yapıcı| Tanım|
| :- | :- |
| [LoadOptions()](/cells/tr/python-net/aspose.cells/loadoptions/__init__/#) | Dosyayı yükleme seçeneklerini oluşturur.|
| [LoadOptions(load_format)](/cells/tr/python-net/aspose.cells/loadoptions/__init__/#LoadFormat) | Dosyayı yükleme seçeneklerini oluşturur.|


###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [load_format](/cells/tr/python-net/aspose.cells/loadoptions/load_format) | Yükleme biçimini alır.|
| [password](/cells/tr/python-net/aspose.cells/loadoptions/password) | Çalışma kitabının parolasını alır ve ayarlar.|
| [parsing_formula_on_open](/cells/tr/python-net/aspose.cells/loadoptions/parsing_formula_on_open) | Dosyayı okurken formülün ayrıştırılıp ayrıştırılmadığını gösterir.|
| [parsing_pivot_cached_records](/cells/tr/python-net/aspose.cells/loadoptions/parsing_pivot_cached_records) | Dosya yüklenirken özet önbelleğe alınan kayıtların ayrıştırılıp ayrıştırılmayacağını gösterir.<br/> Varsayılan değer yanlıştır.|
| [language_code](/cells/tr/python-net/aspose.cells/loadoptions/language_code) | Dosyayı kaydeden CountryCode'a dayalı olarak Çalışma Kitabı sürümünün kullanıcı arabirimi dilini alır veya ayarlar.|
| [region](/cells/tr/python-net/aspose.cells/loadoptions/region) | Dosyanın yüklendiği andaki CountryCode'a göre sistem bölgesel ayarlarını alır veya ayarlar.|
| [default_style_settings](/cells/tr/python-net/aspose.cells/loadoptions/default_style_settings) | Çalışma kitabının stillerini başlatmak için varsayılan stil ayarlarını alır|
| [standard_font](/cells/tr/python-net/aspose.cells/loadoptions/standard_font) | Varsayılan standart yazı tipi adını ayarlar|
| [standard_font_size](/cells/tr/python-net/aspose.cells/loadoptions/standard_font_size) | Varsayılan standart yazı tipi boyutunu ayarlar.|
| [interrupt_monitor](/cells/tr/python-net/aspose.cells/loadoptions/interrupt_monitor) | Kesme monitörünü alır ve ayarlar.|
| [ignore_not_printed](/cells/tr/python-net/aspose.cells/loadoptions/ignore_not_printed) | Dosya doğrudan yazdırılıyorsa yazdırılmayan verileri yok sayın|
| [check_data_valid](/cells/tr/python-net/aspose.cells/loadoptions/check_data_valid) |Verilerin şablon dosyasında geçerli olup olmadığını kontrol edin.|
| [check_excel_restriction](/cells/tr/python-net/aspose.cells/loadoptions/check_excel_restriction) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde excel dosyasının kısıtlamasının kontrol edilip edilmeyeceği.<br/>Örneğin, excel 32K'dan daha uzun bir dizi değeri girilmesine izin vermez.<br/>Cell.PutValue(string) gibi 32K'dan uzun bir değer girdiğinizde, bu özellik doğruysa, bir İstisna alırsınız.<br/>Bu özellik yanlışsa, giriş dizesi değerinizi hücrenin değeri olarak kabul edeceğiz, böylece daha sonra<br/>CSV gibi diğer dosya formatları için tam dizi değerinin çıktısını alabilirsiniz.<br/>Ancak excel dosya formatı için geçersiz olan bir değer belirlediyseniz,<br/> çalışma kitabını daha sonra excel dosya formatında kaydetmemelisiniz. Aksi halde oluşturulan excel dosyasında beklenmeyen bir hata olabilir.|
| [keep_unparsed_data](/cells/tr/python-net/aspose.cells/loadoptions/keep_unparsed_data) | Şablon dosyasından yüklendiğinde Çalışma Kitabı için ayrıştırılmamış verilerin bellekte tutulup tutulmadığı. Varsayılan doğrudur.|
| [load_filter](/cells/tr/python-net/aspose.cells/loadoptions/load_filter) | Verilerin nasıl yükleneceğini gösteren filtre.|
| [light_cells_data_handler](/cells/tr/python-net/aspose.cells/loadoptions/light_cells_data_handler) | Şablon dosyasını okurken hücre verilerini işlemek için veri işleyici.|
| [memory_setting](/cells/tr/python-net/aspose.cells/loadoptions/memory_setting) | Bellek kullanım seçeneklerini alır veya ayarlar.|
| [warning_callback](/cells/tr/python-net/aspose.cells/loadoptions/warning_callback) | Uyarı geri aramasını alır veya ayarlar.|
| [auto_fitter_options](/cells/tr/python-net/aspose.cells/loadoptions/auto_fitter_options) | Otomatik fitre seçeneklerini alır ve ayarlar|
| [auto_filter](/cells/tr/python-net/aspose.cells/loadoptions/auto_filter) | Dosyaları yüklerken verilerin otomatik olarak filtrelenip filtrelenmediğini gösterir.|
| [font_configs](/cells/tr/python-net/aspose.cells/loadoptions/font_configs) | Bireysel yazı tipi yapılandırmalarını alır ve ayarlar.<br/> Yalnızca yüklemek için bu [LoadOptions](/cells/tr/python-net/aspose.cells/loadoptions)'i kullanan [Workbook](/cells/tr/python-net/aspose.cells/workbook) için çalışır.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [set_paper_size(type)](/cells/tr/python-net/aspose.cells/loadoptions/set_paper_size/#PaperSizeType) | Varsayılan yazıcı ayarından varsayılan yazdırma kağıdı boyutunu ayarlar.|



###  Ayrıca bakınız
* modül [aspose.cells](..)
* sınıf [LoadOptions](/cells/tr/python-net/aspose.cells/loadoptions)
* sınıf [Workbook](/cells/tr/python-net/aspose.cells/workbook)
