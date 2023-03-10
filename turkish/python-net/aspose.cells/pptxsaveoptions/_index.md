---
title: PptxSaveOptions sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 1190
url: /tr/python-net/aspose.cells/pptxsaveoptions/
is_root: false
---
##  PptxSaveOptions sınıfı
Pptx kaydetme seçeneklerini temsil eder.



**Miras:** [PptxSaveOptions](/cells/python-net/aspose.cells/pptxsaveoptions) → 
[PaginatedSaveOptions](/cells/python-net/aspose.cells/paginatedsaveoptions) → 
[SaveOptions](/cells/tr/python-net/aspose.cells/saveoptions)



PptxSaveOptions türü aşağıdaki üyeleri gösterir:

###  İnşaatçılar
| Yapıcı| Tanım|
| :- | :- |
| [PptxSaveOptions()](/cells/tr/python-net/aspose.cells/pptxsaveoptions/__init__/#) | Pptx kaydetme seçeneklerini temsil eder.|
| [PptxSaveOptions(save_as_image)](/cells/tr/python-net/aspose.cells/pptxsaveoptions/__init__/#bool) | .pptx dosyasını kaydetme seçeneklerini temsil eder.|


###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [save_format](/cells/tr/python-net/aspose.cells/pptxsaveoptions/save_format) | Kayıt dosyası formatını alır.|
| [clear_data](/cells/tr/python-net/aspose.cells/pptxsaveoptions/clear_data) | Dosyayı kaydettikten sonra çalışma kitabını boşaltın.|
| [cached_file_folder](/cells/tr/python-net/aspose.cells/pptxsaveoptions/cached_file_folder) | Önbelleğe alınmış dosya klasörü, bazı büyük verileri depolamak için kullanılır.|
| [validate_merged_areas](/cells/tr/python-net/aspose.cells/pptxsaveoptions/validate_merged_areas) | Dosyayı kaydetmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmadığını gösterir.|
| [merge_areas](/cells/tr/python-net/aspose.cells/pptxsaveoptions/merge_areas) | Dosyayı kaydetmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmediğini belirtir.|
| [create_directory](/cells/tr/python-net/aspose.cells/pptxsaveoptions/create_directory) | true ise ve dizin yoksa, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur.|
| [sort_names](/cells/tr/python-net/aspose.cells/pptxsaveoptions/sort_names) | Dosyayı kaydetmeden önce tanımlı adların sıralanıp sıralanmadığını gösterir.|
| [sort_external_names](/cells/tr/python-net/aspose.cells/pptxsaveoptions/sort_external_names) |Dosyayı kaydetmeden önce harici tanımlı adların sıralanıp sıralanmadığını gösterir.|
| [refresh_chart_cache](/cells/tr/python-net/aspose.cells/pptxsaveoptions/refresh_chart_cache) | Grafik önbellek verilerinin yenilenip yenilenmediğini gösterir.|
| [warning_callback](/cells/tr/python-net/aspose.cells/pptxsaveoptions/warning_callback) | Uyarı geri aramasını alır veya ayarlar.|
| [update_smart_art](/cells/tr/python-net/aspose.cells/pptxsaveoptions/update_smart_art) | Akıllı sanat ayarının güncellenip güncellenmediğini gösterir.<br/> Varsayılan değer yanlıştır.|
| [default_font](/cells/tr/python-net/aspose.cells/pptxsaveoptions/default_font) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipiyle ayarlanmadığında,<br/>Pdf, görüntüde blok olarak görünebilirler.<br/>Bu karakterleri göstermek için MingLiu veya MS Gothic gibi bir Varsayılan Yazı Tipi ayarlayın.<br/> Bu özellik ayarlanmazsa, Aspose.Cells, bu unicode karakterleri göstermek için sistem varsayılan yazı tipini kullanır.|
| [check_workbook_default_font](/cells/tr/python-net/aspose.cells/pptxsaveoptions/check_workbook_default_font) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipiyle ayarlanmadığında,<br/>Pdf, görüntüde blok olarak görünebilirler.<br/> Önce bu karakterleri göstermek için çalışma kitabının varsayılan yazı tipini kullanmayı denemek için bunu true olarak ayarlayın.|
| [check_font_compatibility](/cells/tr/python-net/aspose.cells/pptxsaveoptions/check_font_compatibility) |Metindeki her karakter için yazı tipi uyumluluğunun kontrol edilip edilmeyeceğini belirtir.|
| [is_font_substitution_char_granularity](/cells/tr/python-net/aspose.cells/pptxsaveoptions/is_font_substitution_char_granularity) | Yalnızca hücre yazı tipi uyumlu olmadığında karakter yazı tipinin değiştirilip değiştirilmeyeceğini belirtir.|
| [one_page_per_sheet](/cells/tr/python-net/aspose.cells/pptxsaveoptions/one_page_per_sheet) | OnePagePerSheet true ise, sonuçta bir sayfanın tüm içeriği yalnızca bir sayfaya çıkar.<br/> pagesetup'ın kağıt boyutu geçersiz olacak ve pagesetup'ın diğer ayarları geçersiz olacaktır.<br/> yine de geçerli olacaktır.|
| [all_columns_in_one_page_per_sheet](/cells/tr/python-net/aspose.cells/pptxsaveoptions/all_columns_in_one_page_per_sheet) | AllColumnsInOnePagePerSheet true olursa, bir sayfanın tüm sütun içeriği sonuçta yalnızca bir sayfaya çıkar.<br/> pagesetup'ın kağıt boyutunun genişliği dikkate alınmaz ve pagesetup'ın diğer ayarları dikkate alınmaz.<br/> yine de geçerli olacaktır.|
| [ignore_error](/cells/tr/python-net/aspose.cells/pptxsaveoptions/ignore_error) | İşleme sırasında hatayı gizlemeniz gerekip gerekmediğini gösterir.<br/> Hata şekil, görüntü, grafik oluşturma vb. hata olabilir.|
| [output_blank_page_when_nothing_to_print](/cells/tr/python-net/aspose.cells/pptxsaveoptions/output_blank_page_when_nothing_to_print) | Yazdırılacak bir şey olmadığında boş bir sayfa çıktısı alınıp alınmayacağını belirtir.|
| [page_index](/cells/tr/python-net/aspose.cells/pptxsaveoptions/page_index) | Kaydedilecek ilk sayfanın 0 tabanlı dizinini alır veya ayarlar.|
| [page_count](/cells/tr/python-net/aspose.cells/pptxsaveoptions/page_count) | Kaydedilecek sayfa sayısını alır veya ayarlar.|
| [printing_page_type](/cells/tr/python-net/aspose.cells/pptxsaveoptions/printing_page_type) | Hangi sayfaların yazdırılmayacağını belirtir.|
| [gridline_type](/cells/tr/python-net/aspose.cells/pptxsaveoptions/gridline_type) | Kılavuz çizgisi türünü alır veya ayarlar.|
| [text_cross_type](/cells/tr/python-net/aspose.cells/pptxsaveoptions/text_cross_type) | Metin genişliği hücre genişliğinden büyük olduğunda görüntülenen metin türünü alır veya ayarlar.|
| [default_edit_language](/cells/tr/python-net/aspose.cells/pptxsaveoptions/default_edit_language) | Varsayılan düzenleme dilini alır veya ayarlar.|
| [sheet_set](/cells/tr/python-net/aspose.cells/pptxsaveoptions/sheet_set) |İşlenecek sayfaları alır veya ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: [SheetSet.visible](/cells/tr/python-net/aspose.cells.rendering/sheetset#visible).|
| [draw_object_event_handler](/cells/tr/python-net/aspose.cells/pptxsaveoptions/draw_object_event_handler) | İşleme sırasında DrawObject ve Bound'u almak için bu arabirimi uygular.|
| [page_saving_callback](/cells/tr/python-net/aspose.cells/pptxsaveoptions/page_saving_callback) | Sayfa kaydetme işleminin ilerleyişini kontrol edin/gösterin.|



###  Ayrıca bakınız
* modül [aspose.cells](..)
* sınıf [PaginatedSaveOptions](/cells/tr/python-net/aspose.cells/paginatedsaveoptions)
* sınıf [PptxSaveOptions](/cells/tr/python-net/aspose.cells/pptxsaveoptions)
* sınıf [SaveOptions](/cells/tr/python-net/aspose.cells/saveoptions)
