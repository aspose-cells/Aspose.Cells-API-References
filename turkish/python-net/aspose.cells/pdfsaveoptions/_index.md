---
title: PdfSaveOptions sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 1180
url: /tr/python-net/aspose.cells/pdfsaveoptions/
is_root: false
---
##  PdfSaveOptions sınıf
Pdf dosyasını kaydetme seçeneklerini temsil eder.



**Miras:** [PdfSaveOptions](/cells/python-net/aspose.cells/pdfsaveoptions) → 
[PaginatedSaveOptions](/cells/python-net/aspose.cells/paginatedsaveoptions) → 
[SaveOptions](/cells/tr/python-net/aspose.cells/saveoptions)



PdfSaveOptions türü aşağıdaki üyeleri gösterir:

###  İnşaatçılar
| Yapıcı| Tanım|
| :- | :- |
| [PdfSaveOptions()](/cells/tr/python-net/aspose.cells/pdfsaveoptions/__init__/#) | Pdf dosyasını kaydetme seçeneklerini oluşturur.|


###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [save_format](/cells/tr/python-net/aspose.cells/pdfsaveoptions/save_format) | Kayıt dosyası formatını alır.|
| [clear_data](/cells/tr/python-net/aspose.cells/pdfsaveoptions/clear_data) | Dosyayı kaydettikten sonra çalışma kitabını boşaltın.|
| [cached_file_folder](/cells/tr/python-net/aspose.cells/pdfsaveoptions/cached_file_folder) | Önbelleğe alınmış dosya klasörü, bazı büyük verileri depolamak için kullanılır.|
| [validate_merged_areas](/cells/tr/python-net/aspose.cells/pdfsaveoptions/validate_merged_areas) | Dosyayı kaydetmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmadığını gösterir.|
| [merge_areas](/cells/tr/python-net/aspose.cells/pdfsaveoptions/merge_areas) | Dosyayı kaydetmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmediğini belirtir.|
| [create_directory](/cells/tr/python-net/aspose.cells/pdfsaveoptions/create_directory) | true ise ve dizin yoksa, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur.|
| [sort_names](/cells/tr/python-net/aspose.cells/pdfsaveoptions/sort_names) | Dosyayı kaydetmeden önce tanımlı adların sıralanıp sıralanmadığını gösterir.|
| [sort_external_names](/cells/tr/python-net/aspose.cells/pdfsaveoptions/sort_external_names) | Dosyayı kaydetmeden önce harici tanımlı adların sıralanıp sıralanmadığını gösterir.|
| [refresh_chart_cache](/cells/tr/python-net/aspose.cells/pdfsaveoptions/refresh_chart_cache) |Grafik önbellek verilerinin yenilenip yenilenmediğini gösterir.|
| [warning_callback](/cells/tr/python-net/aspose.cells/pdfsaveoptions/warning_callback) | Uyarı geri aramasını alır veya ayarlar.|
| [update_smart_art](/cells/tr/python-net/aspose.cells/pdfsaveoptions/update_smart_art) | Akıllı sanat ayarının güncellenip güncellenmediğini gösterir.<br/> Varsayılan değer yanlıştır.|
| [default_font](/cells/tr/python-net/aspose.cells/pdfsaveoptions/default_font) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipiyle ayarlanmadığında,<br/>Pdf, görüntüde blok olarak görünebilirler.<br/>Bu karakterleri göstermek için MingLiu veya MS Gothic gibi bir Varsayılan Yazı Tipi ayarlayın.<br/> Bu özellik ayarlanmazsa, Aspose.Cells, bu unicode karakterleri göstermek için sistem varsayılan yazı tipini kullanır.|
| [check_workbook_default_font](/cells/tr/python-net/aspose.cells/pdfsaveoptions/check_workbook_default_font) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipiyle ayarlanmadığında,<br/>Pdf, görüntüde blok olarak görünebilirler.<br/> Önce bu karakterleri göstermek için çalışma kitabının varsayılan yazı tipini kullanmayı denemek için bunu true olarak ayarlayın.|
| [check_font_compatibility](/cells/tr/python-net/aspose.cells/pdfsaveoptions/check_font_compatibility) | Metindeki her karakter için yazı tipi uyumluluğunun kontrol edilip edilmeyeceğini belirtir.|
| [is_font_substitution_char_granularity](/cells/tr/python-net/aspose.cells/pdfsaveoptions/is_font_substitution_char_granularity) | Yalnızca hücre yazı tipi uyumlu olmadığında karakter yazı tipinin değiştirilip değiştirilmeyeceğini belirtir.|
| [one_page_per_sheet](/cells/tr/python-net/aspose.cells/pdfsaveoptions/one_page_per_sheet) | OnePagePerSheet true ise, sonuçta bir sayfanın tüm içeriği yalnızca bir sayfaya çıkar.<br/> pagesetup'ın kağıt boyutu geçersiz olacak ve pagesetup'ın diğer ayarları geçersiz olacaktır.<br/> yine de geçerli olacaktır.|
| [all_columns_in_one_page_per_sheet](/cells/tr/python-net/aspose.cells/pdfsaveoptions/all_columns_in_one_page_per_sheet) | AllColumnsInOnePagePerSheet true olursa, bir sayfanın tüm sütun içeriği sonuçta yalnızca bir sayfaya çıkar.<br/> pagesetup'ın kağıt boyutunun genişliği dikkate alınmaz ve pagesetup'ın diğer ayarları dikkate alınmaz.<br/> yine de geçerli olacaktır.|
| [ignore_error](/cells/tr/python-net/aspose.cells/pdfsaveoptions/ignore_error) | İşleme sırasında hatayı gizlemeniz gerekip gerekmediğini gösterir.<br/> Hata şekil, görüntü, grafik oluşturma vb. hata olabilir.|
| [output_blank_page_when_nothing_to_print](/cells/tr/python-net/aspose.cells/pdfsaveoptions/output_blank_page_when_nothing_to_print) | Yazdırılacak bir şey olmadığında boş bir sayfa çıktısı alınıp alınmayacağını belirtir.|
| [page_index](/cells/tr/python-net/aspose.cells/pdfsaveoptions/page_index) | Kaydedilecek ilk sayfanın 0 tabanlı dizinini alır veya ayarlar.|
| [page_count](/cells/tr/python-net/aspose.cells/pdfsaveoptions/page_count) | Kaydedilecek sayfa sayısını alır veya ayarlar.|
| [printing_page_type](/cells/tr/python-net/aspose.cells/pdfsaveoptions/printing_page_type) | Hangi sayfaların yazdırılmayacağını belirtir.|
| [gridline_type](/cells/tr/python-net/aspose.cells/pdfsaveoptions/gridline_type) | Kılavuz çizgisi türünü alır veya ayarlar.|
| [text_cross_type](/cells/tr/python-net/aspose.cells/pdfsaveoptions/text_cross_type) | Metin genişliği hücre genişliğinden büyük olduğunda görüntülenen metin türünü alır veya ayarlar.|
| [default_edit_language](/cells/tr/python-net/aspose.cells/pdfsaveoptions/default_edit_language) | Varsayılan düzenleme dilini alır veya ayarlar.|
| [sheet_set](/cells/tr/python-net/aspose.cells/pdfsaveoptions/sheet_set) |İşlenecek sayfaları alır veya ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: [SheetSet.visible](/cells/tr/python-net/aspose.cells.rendering/sheetset#visible).|
| [draw_object_event_handler](/cells/tr/python-net/aspose.cells/pdfsaveoptions/draw_object_event_handler) | İşleme sırasında DrawObject ve Bound'u almak için bu arabirimi uygular.|
| [page_saving_callback](/cells/tr/python-net/aspose.cells/pdfsaveoptions/page_saving_callback) |Sayfa kaydetme işleminin ilerleyişini kontrol edin/gösterin.|
| [embed_standard_windows_fonts](/cells/tr/python-net/aspose.cells/pdfsaveoptions/embed_standard_windows_fonts) | Gerçek tip yazı tiplerini gömmek için doğru.<br/>Yalnızca ASCII karakterleri 32-127'yi etkiler.<br/>127'den büyük karakter kodları için yazı tipleri her zaman gömülüdür.<br/>Yazı tipleri her zaman PDF/A-1a, PDF/A-1b standardı için gömülüdür.<br/> Varsayılan doğrudur.|
| [bookmark](/cells/tr/python-net/aspose.cells/pdfsaveoptions/bookmark) | [PdfBookmarkEntry](/cells/tr/python-net/aspose.cells.rendering/pdfbookmarkentry) nesnesini alır ve ayarlar.|
| [compliance](/cells/tr/python-net/aspose.cells/pdfsaveoptions/compliance) | Çalışma kitabı bu özellikte PdfCompliance'a göre pdf'ye dönüştürülür.|
| [security_options](/cells/tr/python-net/aspose.cells/pdfsaveoptions/security_options) | xls2pdf sonucunda güvenlik gerektiğinde bu seçenekleri ayarlayın.|
| [image_type](/cells/tr/python-net/aspose.cells/pdfsaveoptions/image_type) | Grafiği ve şekli dönüştürürken görüntü tipini temsil eder.|
| [calculate_formula](/cells/tr/python-net/aspose.cells/pdfsaveoptions/calculate_formula) | PDF dosyasını kaydetmeden önce formüllerin hesaplanıp hesaplanmayacağını belirtir.|
| [pdf_compression](/cells/tr/python-net/aspose.cells/pdfsaveoptions/pdf_compression) |Sıkıştırma algoritmasını belirtin|
| [created_time](/cells/tr/python-net/aspose.cells/pdfsaveoptions/created_time) | Pdf belgesi oluşturma zamanını alır ve ayarlar.|
| [producer](/cells/tr/python-net/aspose.cells/pdfsaveoptions/producer) | Oluşturulan pdf belgesinin üreticisini alır ve ayarlar.|
| [optimization_type](/cells/tr/python-net/aspose.cells/pdfsaveoptions/optimization_type) | Pdf optimizasyon türünü alır ve ayarlar.|
| [custom_properties_export](/cells/tr/python-net/aspose.cells/pdfsaveoptions/custom_properties_export) | [CustomDocumentPropertyCollection](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection)'in PDF dosyasına nasıl aktarılacağını belirleyen bir değer alır veya ayarlar. Varsayılan değer Yok'tur.|
| [export_document_structure](/cells/tr/python-net/aspose.cells/pdfsaveoptions/export_document_structure) | Belge yapısının dışa aktarılıp aktarılmayacağını belirtir.|
| [emf_render_setting](/cells/tr/python-net/aspose.cells/pdfsaveoptions/emf_render_setting) | Emf meta dosyasını işlemek için ayar.|
| [display_doc_title](/cells/tr/python-net/aspose.cells/pdfsaveoptions/display_doc_title) | Pencerenin başlık çubuğunun belge başlığını gösterip göstermeyeceğini belirtir.|
| [font_encoding](/cells/tr/python-net/aspose.cells/pdfsaveoptions/font_encoding) | Pdf'de gömülü yazı tipi kodlamasını alır veya ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [set_image_resample(desired_ppi, jpeg_quality)](/cells/tr/python-net/aspose.cells/pdfsaveoptions/set_image_resample/#int-int) | Yeniden örnekleme görüntüleri ve jpeg kalitesinin istenen ÜFE'sini (piksel/inç) ayarlar.<br/> Tüm resimler belirtilen kalite ayarıyla JPEG'e dönüştürülecek,<br/>ve belirtilen ÜFE'den (inç başına piksel) daha büyük olan resimler yeniden örneklenir.|



###  Ayrıca bakınız
* modül [aspose.cells](..)
* sınıf [CustomDocumentPropertyCollection](/cells/tr/python-net/aspose.cells.properties/customdocumentpropertycollection)
* sınıf [PaginatedSaveOptions](/cells/tr/python-net/aspose.cells/paginatedsaveoptions)
* sınıf [PdfBookmarkEntry](/cells/tr/python-net/aspose.cells.rendering/pdfbookmarkentry)
* sınıf [PdfSaveOptions](/cells/tr/python-net/aspose.cells/pdfsaveoptions)
* sınıf [SaveOptions](/cells/tr/python-net/aspose.cells/saveoptions)
