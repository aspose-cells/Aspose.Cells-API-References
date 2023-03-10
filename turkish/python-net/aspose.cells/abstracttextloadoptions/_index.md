---
title: AbstractTextLoadOptions sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 60
url: /tr/python-net/aspose.cells/abstracttextloadoptions/
is_root: false
---
##  AbstractTextLoadOptions sınıfı
Metin değerleri yüklemek için yaygın seçenekler



**Miras:** [AbstractTextLoadOptions](/cells/python-net/aspose.cells/abstracttextloadoptions) → 
[LoadOptions](/cells/tr/python-net/aspose.cells/loadoptions)



AbstractTextLoadOptions türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [load_format](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/load_format) | Yükleme biçimini alır.|
| [password](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/password) | Çalışma kitabının parolasını alır ve ayarlar.|
| [parsing_formula_on_open](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/parsing_formula_on_open) | Dosyayı okurken formülün ayrıştırılıp ayrıştırılmadığını gösterir.|
| [parsing_pivot_cached_records](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/parsing_pivot_cached_records) | Dosya yüklenirken özet önbelleğe alınan kayıtların ayrıştırılıp ayrıştırılmayacağını gösterir.<br/> Varsayılan değer yanlıştır.|
| [language_code](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/language_code) | Dosyayı kaydeden CountryCode'a dayalı olarak Çalışma Kitabı sürümünün kullanıcı arabirimi dilini alır veya ayarlar.|
| [region](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/region) | Dosyanın yüklendiği andaki CountryCode'a göre sistem bölgesel ayarlarını alır veya ayarlar.|
| [default_style_settings](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/default_style_settings) | Çalışma kitabının stillerini başlatmak için varsayılan stil ayarlarını alır|
| [standard_font](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/standard_font) | Varsayılan standart yazı tipi adını ayarlar|
| [standard_font_size](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/standard_font_size) | Varsayılan standart yazı tipi boyutunu ayarlar.|
| [interrupt_monitor](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/interrupt_monitor) | Kesme monitörünü alır ve ayarlar.|
| [ignore_not_printed](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/ignore_not_printed) | Dosya doğrudan yazdırılıyorsa yazdırılmayan verileri yok sayın|
| [check_data_valid](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/check_data_valid) |Verilerin şablon dosyasında geçerli olup olmadığını kontrol edin.|
| [check_excel_restriction](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/check_excel_restriction) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde excel dosyasının kısıtlamasının kontrol edilip edilmeyeceği.<br/>Örneğin, excel 32K'dan daha uzun bir dizi değeri girilmesine izin vermez.<br/>Cell.PutValue(string) gibi 32K'dan uzun bir değer girdiğinizde, bu özellik doğruysa, bir İstisna alırsınız.<br/>Bu özellik yanlışsa, giriş dizesi değerinizi hücrenin değeri olarak kabul edeceğiz, böylece daha sonra<br/>CSV gibi diğer dosya formatları için tam dizi değerinin çıktısını alabilirsiniz.<br/>Ancak excel dosya formatı için geçersiz olan bir değer belirlediyseniz,<br/> çalışma kitabını daha sonra excel dosya formatında kaydetmemelisiniz. Aksi halde oluşturulan excel dosyasında beklenmeyen bir hata olabilir.|
| [keep_unparsed_data](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/keep_unparsed_data) | Şablon dosyasından yüklendiğinde Çalışma Kitabı için ayrıştırılmamış verilerin bellekte tutulup tutulmadığı. Varsayılan doğrudur.|
| [load_filter](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/load_filter) | Verilerin nasıl yükleneceğini gösteren filtre.|
| [light_cells_data_handler](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/light_cells_data_handler) | Şablon dosyasını okurken hücre verilerini işlemek için veri işleyici.|
| [memory_setting](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/memory_setting) | Bellek kullanım seçeneklerini alır veya ayarlar.|
| [warning_callback](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/warning_callback) | Uyarı geri aramasını alır veya ayarlar.|
| [auto_fitter_options](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/auto_fitter_options) | Otomatik fitre seçeneklerini alır ve ayarlar|
| [auto_filter](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/auto_filter) | Dosyaları yüklerken verilerin otomatik olarak filtrelenip filtrelenmediğini gösterir.|
| [font_configs](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/font_configs) | Bireysel yazı tipi yapılandırmalarını alır ve ayarlar.<br/> Yalnızca yüklemek için bu [LoadOptions](/cells/tr/python-net/aspose.cells/loadoptions)'i kullanan [Workbook](/cells/tr/python-net/aspose.cells/workbook) için çalışır.|
| [encoding](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/encoding) | Varsayılan kodlamayı alır ve ayarlar. Yalnızca csv dosyası için geçerlidir.|
| [load_style_strategy](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/load_style_strategy) |Dize değerini sayıya veya tarih saatine dönüştürürken ayrıştırılmış değerler için stil uygulama stratejisini belirtir.|
| [convert_numeric_data](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/convert_numeric_data) | Metin dosyasındaki dizenin sayısal verilere dönüştürülüp dönüştürülmediğini gösteren bir değer alır veya ayarlar.|
| [convert_date_time_data](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/convert_date_time_data) | Metin dosyasındaki dizenin tarih verilerine dönüştürülüp dönüştürülmediğini gösteren bir değer alır veya ayarlar.|
| [keep_precision](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/keep_precision) | Uzunluk 15 ise bir dize değerinin ayrıştırılıp ayrıştırılmayacağını gösterir.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [set_paper_size(type)](/cells/tr/python-net/aspose.cells/abstracttextloadoptions/set_paper_size/#PaperSizeType) | Varsayılan yazıcı ayarından varsayılan yazdırma kağıdı boyutunu ayarlar.|



###  Ayrıca bakınız
* modül [aspose.cells](..)
* sınıf [AbstractTextLoadOptions](/cells/tr/python-net/aspose.cells/abstracttextloadoptions)
* sınıf [LoadOptions](/cells/tr/python-net/aspose.cells/loadoptions)
* sınıf [Workbook](/cells/tr/python-net/aspose.cells/workbook)
