---
title: TxtSaveOptions sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 1520
url: /tr/python-net/aspose.cells/txtsaveoptions/
is_root: false
---
##  TxtSaveOptions sınıfı
CSV/sekmeyle ayrılmış/diğer metin biçimi için kaydetme seçeneklerini temsil eder.



**Miras:** [TxtSaveOptions](/cells/python-net/aspose.cells/txtsaveoptions) → 
[SaveOptions](/cells/tr/python-net/aspose.cells/saveoptions)



TxtSaveOptions türü aşağıdaki üyeleri gösterir:

###  İnşaatçılar
| Yapıcı| Tanım|
| :- | :- |
| [TxtSaveOptions()](/cells/tr/python-net/aspose.cells/txtsaveoptions/__init__/#) | Metin dosyası kaydetme seçenekleri oluşturur.|
| [TxtSaveOptions(format)](/cells/tr/python-net/aspose.cells/txtsaveoptions/__init__/#SaveFormat) | Metin dosyası kaydetme seçenekleri oluşturur.|


###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [save_format](/cells/tr/python-net/aspose.cells/txtsaveoptions/save_format) | Kayıt dosyası formatını alır.|
| [clear_data](/cells/tr/python-net/aspose.cells/txtsaveoptions/clear_data) | Dosyayı kaydettikten sonra çalışma kitabını boşaltın.|
| [cached_file_folder](/cells/tr/python-net/aspose.cells/txtsaveoptions/cached_file_folder) | Önbelleğe alınmış dosya klasörü, bazı büyük verileri depolamak için kullanılır.|
| [validate_merged_areas](/cells/tr/python-net/aspose.cells/txtsaveoptions/validate_merged_areas) | Dosyayı kaydetmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmadığını gösterir.|
| [merge_areas](/cells/tr/python-net/aspose.cells/txtsaveoptions/merge_areas) | Dosyayı kaydetmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmediğini belirtir.|
| [create_directory](/cells/tr/python-net/aspose.cells/txtsaveoptions/create_directory) | true ise ve dizin yoksa, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur.|
| [sort_names](/cells/tr/python-net/aspose.cells/txtsaveoptions/sort_names) | Dosyayı kaydetmeden önce tanımlı adların sıralanıp sıralanmadığını gösterir.|
| [sort_external_names](/cells/tr/python-net/aspose.cells/txtsaveoptions/sort_external_names) |Dosyayı kaydetmeden önce harici tanımlı adların sıralanıp sıralanmadığını gösterir.|
| [refresh_chart_cache](/cells/tr/python-net/aspose.cells/txtsaveoptions/refresh_chart_cache) | Grafik önbellek verilerinin yenilenip yenilenmediğini gösterir.|
| [warning_callback](/cells/tr/python-net/aspose.cells/txtsaveoptions/warning_callback) | Uyarı geri aramasını alır veya ayarlar.|
| [update_smart_art](/cells/tr/python-net/aspose.cells/txtsaveoptions/update_smart_art) | Akıllı sanat ayarının güncellenip güncellenmediğini gösterir.<br/> Varsayılan değer yanlıştır.|
| [separator](/cells/tr/python-net/aspose.cells/txtsaveoptions/separator) | Metin dosyasının char Sınırlayıcısını alır ve ayarlar.|
| [separator_string](/cells/tr/python-net/aspose.cells/txtsaveoptions/separator_string) | Ayırıcı olarak bir dize değeri alır ve ayarlar.|
| [encoding](/cells/tr/python-net/aspose.cells/txtsaveoptions/encoding) | Varsayılan kodlamayı alır ve ayarlar.|
| [always_quoted](/cells/tr/python-net/aspose.cells/txtsaveoptions/always_quoted) | Her alan için her zaman ''' eklenip eklenmeyeceğini belirtir.<br/>true ise, tüm değerler alıntılanacaktır;<br/>false ise, değerler yalnızca gerektiğinde alıntılanır (örneğin,<br/>değerler '"' , '\n' veya ayırıcı karakter gibi özel karakterler içerdiğinde).<br/> Varsayılan yanlıştır.|
| [quote_type](/cells/tr/python-net/aspose.cells/txtsaveoptions/quote_type) | Dışa aktarılan metin dosyasında değerlerin nasıl alıntılanacağını alır veya ayarlar.|
| [format_strategy](/cells/tr/python-net/aspose.cells/txtsaveoptions/format_strategy) | Hücre değerini dize olarak dışa aktarırken biçim stratejisini alır ve ayarlar.|
| [light_cells_data_provider](/cells/tr/python-net/aspose.cells/txtsaveoptions/light_cells_data_provider) | Veri sağlayıcı, çalışma kitabını hafif modda kaydetmek için hücrelere veri sağlar.|
| [trim_leading_blank_row_and_column](/cells/tr/python-net/aspose.cells/txtsaveoptions/trim_leading_blank_row_and_column) | Öndeki boş satırların ve sütunların MS Excel'in yaptığı gibi kırpılıp kırpılmayacağını belirtir.<br/> Varsayılan doğrudur.|
| [trim_tailing_blank_cells](/cells/tr/python-net/aspose.cells/txtsaveoptions/trim_tailing_blank_cells) | Bir satırdaki kuyruk boş hücrelerinin kırpılıp kırpılmayacağını belirtir. Varsayılan yanlıştır.|
| [keep_separators_for_blank_row](/cells/tr/python-net/aspose.cells/txtsaveoptions/keep_separators_for_blank_row) | Boş satır için ayırıcıların gösterilmesi gerekip gerekmediğini gösterir.<br/> Varsayılan değer yanlıştır, bu nedenle varsayılan olarak boş satırın içeriği boş olacaktır.|
| [export_area](/cells/tr/python-net/aspose.cells/txtsaveoptions/export_area) | Dışa aktarılacak hücre aralığı.|
| [export_quote_prefix](/cells/tr/python-net/aspose.cells/txtsaveoptions/export_quote_prefix) | Tek tırnak işaretinin bir hücrenin değerinin parçası olarak dışa aktarılıp aktarılmayacağını belirtir<br/> [Style.quote_prefix](/cells/tr/python-net/aspose.cells/style#quote_prefix) bunun için doğru olduğunda. Varsayılan yanlıştır.|
| [export_all_sheets](/cells/tr/python-net/aspose.cells/txtsaveoptions/export_all_sheets) |Tüm sayfaların metin dosyasına aktarılıp aktarılmadığını gösterir.<br/> Yanlışsa, tıpkı MS Excel gibi yalnızca aktif sayfayı dışa aktarın.|



###  Ayrıca bakınız
* modül [aspose.cells](..)
* sınıf [SaveOptions](/cells/tr/python-net/aspose.cells/saveoptions)
* sınıf [TxtSaveOptions](/cells/tr/python-net/aspose.cells/txtsaveoptions)
