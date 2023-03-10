---
title: NumbersLoadOptions sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 10
url: /tr/python-net/aspose.cells.numbers/numbersloadoptions/
is_root: false
---
##  NumbersLoadOptions sınıfı
Apple Numbers dosyalarını yükleme seçeneklerini temsil eder.



**Miras:** [NumbersLoadOptions](/cells/python-net/aspose.cells.numbers/numbersloadoptions) → 
[LoadOptions](/cells/tr/python-net/aspose.cells/loadoptions)



NumbersLoadOptions türü aşağıdaki üyeleri gösterir:

###  İnşaatçılar
| Yapıcı| Tanım|
| :- | :- |
| [NumbersLoadOptions()](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/__init__/#) | Yapıcı.|


###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [load_format](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/load_format) | Yükleme biçimini alır.|
| [password](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/password) | Çalışma kitabının parolasını alır ve ayarlar.|
| [parsing_formula_on_open](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/parsing_formula_on_open) | Dosyayı okurken formülün ayrıştırılıp ayrıştırılmadığını gösterir.|
| [parsing_pivot_cached_records](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/parsing_pivot_cached_records) | Dosya yüklenirken özet önbelleğe alınan kayıtların ayrıştırılıp ayrıştırılmayacağını gösterir.<br/> Varsayılan değer yanlıştır.|
| [language_code](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/language_code) | Dosyayı kaydeden CountryCode'a dayalı olarak Çalışma Kitabı sürümünün kullanıcı arabirimi dilini alır veya ayarlar.|
| [region](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/region) | Dosyanın yüklendiği andaki CountryCode'a göre sistem bölgesel ayarlarını alır veya ayarlar.|
| [default_style_settings](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/default_style_settings) | Çalışma kitabının stillerini başlatmak için varsayılan stil ayarlarını alır|
| [standard_font](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/standard_font) | Varsayılan standart yazı tipi adını ayarlar|
| [standard_font_size](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/standard_font_size) | Varsayılan standart yazı tipi boyutunu ayarlar.|
| [interrupt_monitor](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/interrupt_monitor) | Kesme monitörünü alır ve ayarlar.|
| [ignore_not_printed](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/ignore_not_printed) | Dosya doğrudan yazdırılıyorsa yazdırılmayan verileri yok sayın|
| [check_data_valid](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/check_data_valid) |Verilerin şablon dosyasında geçerli olup olmadığını kontrol edin.|
| [check_excel_restriction](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/check_excel_restriction) | Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde excel dosyasının kısıtlamasının kontrol edilip edilmeyeceği.<br/>Örneğin, excel 32K'dan daha uzun bir dizi değeri girilmesine izin vermez.<br/>Cell.PutValue(string) gibi 32K'dan uzun bir değer girdiğinizde, bu özellik doğruysa, bir İstisna alırsınız.<br/>Bu özellik yanlışsa, giriş dizesi değerinizi hücrenin değeri olarak kabul edeceğiz, böylece daha sonra<br/>CSV gibi diğer dosya formatları için tam dizi değerinin çıktısını alabilirsiniz.<br/>Ancak excel dosya formatı için geçersiz olan bir değer belirlediyseniz,<br/> çalışma kitabını daha sonra excel dosya formatında kaydetmemelisiniz. Aksi halde oluşturulan excel dosyasında beklenmeyen bir hata olabilir.|
| [keep_unparsed_data](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/keep_unparsed_data) | Şablon dosyasından yüklendiğinde Çalışma Kitabı için ayrıştırılmamış verilerin bellekte tutulup tutulmadığı. Varsayılan doğrudur.|
| [load_filter](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/load_filter) | Verilerin nasıl yükleneceğini gösteren filtre.|
| [light_cells_data_handler](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/light_cells_data_handler) | Şablon dosyasını okurken hücre verilerini işlemek için veri işleyici.|
| [memory_setting](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/memory_setting) | Bellek kullanım seçeneklerini alır veya ayarlar.|
| [warning_callback](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/warning_callback) | Uyarı geri aramasını alır veya ayarlar.|
| [auto_fitter_options](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/auto_fitter_options) | Otomatik fitre seçeneklerini alır ve ayarlar|
| [auto_filter](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/auto_filter) | Dosyaları yüklerken verilerin otomatik olarak filtrelenip filtrelenmediğini gösterir.|
| [font_configs](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/font_configs) | Bireysel yazı tipi yapılandırmalarını alır ve ayarlar.<br/> Yalnızca yüklemek için bu [LoadOptions](/cells/tr/python-net/aspose.cells/loadoptions)'i kullanan [Workbook](/cells/tr/python-net/aspose.cells/workbook) için çalışır.|
| [load_table_type](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/load_table_type) | Tek bir çalışma sayfasına birden çok tablo yükleme türünü alır ve ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [set_paper_size(type)](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions/set_paper_size/#PaperSizeType) | Varsayılan yazıcı ayarından varsayılan yazdırma kağıdı boyutunu ayarlar.|



###  Ayrıca bakınız
* modül [aspose.cells.numbers](..)
* sınıf [LoadOptions](/cells/tr/python-net/aspose.cells/loadoptions)
* sınıf [NumbersLoadOptions](/cells/tr/python-net/aspose.cells.numbers/numbersloadoptions)
* sınıf [Workbook](/cells/tr/python-net/aspose.cells/workbook)
