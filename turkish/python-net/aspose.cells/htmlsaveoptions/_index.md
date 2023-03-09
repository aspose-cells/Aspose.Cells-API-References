---
title: HtmlSaveOptions sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 780
url: /tr/python-net/aspose.cells/htmlsaveoptions/
is_root: false
---
##  HtmlSaveOptions sınıf
Html dosyasını kaydetme seçeneklerini temsil eder.



**Miras:** [HtmlSaveOptions](/cells/python-net/aspose.cells/htmlsaveoptions) → 
[SaveOptions](/cells/tr/python-net/aspose.cells/saveoptions)



HtmlSaveOptions türü aşağıdaki üyeleri gösterir:

###  İnşaatçılar
| Yapıcı| Tanım|
| :- | :- |
| [HtmlSaveOptions()](/cells/tr/python-net/aspose.cells/htmlsaveoptions/__init__/#) | Html dosyasını kaydetmek için seçenekler oluşturur.|
| [HtmlSaveOptions(format)](/cells/tr/python-net/aspose.cells/htmlsaveoptions/__init__/#SaveFormat) | Htm dosyasını kaydetmek için seçenekler oluşturur.|


###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [save_format](/cells/tr/python-net/aspose.cells/htmlsaveoptions/save_format) | Kayıt dosyası formatını alır.|
| [clear_data](/cells/tr/python-net/aspose.cells/htmlsaveoptions/clear_data) | Dosyayı kaydettikten sonra çalışma kitabını boşaltın.|
| [cached_file_folder](/cells/tr/python-net/aspose.cells/htmlsaveoptions/cached_file_folder) | Önbelleğe alınmış dosya klasörü, bazı büyük verileri depolamak için kullanılır.|
| [validate_merged_areas](/cells/tr/python-net/aspose.cells/htmlsaveoptions/validate_merged_areas) | Dosyayı kaydetmeden önce birleştirilmiş hücrelerin doğrulanıp doğrulanmadığını gösterir.|
| [merge_areas](/cells/tr/python-net/aspose.cells/htmlsaveoptions/merge_areas) | Dosyayı kaydetmeden önce koşullu biçimlendirme ve doğrulama alanlarının birleştirilip birleştirilmediğini belirtir.|
| [create_directory](/cells/tr/python-net/aspose.cells/htmlsaveoptions/create_directory) | true ise ve dizin yoksa, dosya kaydedilmeden önce dizin otomatik olarak oluşturulur.|
| [sort_names](/cells/tr/python-net/aspose.cells/htmlsaveoptions/sort_names) | Dosyayı kaydetmeden önce tanımlı adların sıralanıp sıralanmadığını gösterir.|
| [sort_external_names](/cells/tr/python-net/aspose.cells/htmlsaveoptions/sort_external_names) | Dosyayı kaydetmeden önce harici tanımlı adların sıralanıp sıralanmadığını gösterir.|
| [refresh_chart_cache](/cells/tr/python-net/aspose.cells/htmlsaveoptions/refresh_chart_cache) |Grafik önbellek verilerinin yenilenip yenilenmediğini gösterir.|
| [warning_callback](/cells/tr/python-net/aspose.cells/htmlsaveoptions/warning_callback) | Uyarı geri aramasını alır veya ayarlar.|
| [update_smart_art](/cells/tr/python-net/aspose.cells/htmlsaveoptions/update_smart_art) | Akıllı sanat ayarının güncellenip güncellenmediğini gösterir.<br/> Varsayılan değer yanlıştır.|
| [ignore_invisible_shapes](/cells/tr/python-net/aspose.cells/htmlsaveoptions/ignore_invisible_shapes) | Görünmeyen şekillerin dışa aktarılıp aktarılmadığını belirtin|
| [page_title](/cells/tr/python-net/aspose.cells/htmlsaveoptions/page_title) | Html sayfasının başlığı.<br/> Yalnızca html akışına kaydetmek için.|
| [attached_files_directory](/cells/tr/python-net/aspose.cells/htmlsaveoptions/attached_files_directory) |Eklenen dosyaların kaydedileceği dizin.<br/> Yalnızca html akışına kaydetmek için.|
| [attached_files_url_prefix](/cells/tr/python-net/aspose.cells/htmlsaveoptions/attached_files_url_prefix) | Html dosyasındaki resim gibi ekli dosyaların URL önekini belirtin.<br/> Yalnızca html akışına kaydetmek için.|
| [default_font_name](/cells/tr/python-net/aspose.cells/htmlsaveoptions/default_font_name) | Html'yi dışa aktarmak için varsayılan yazı tipi adını belirtin, stil yazı tipi mevcut olmadığında varsayılan yazı tipi kullanılacaktır,<br/>Bu özellik boşsa, Aspose.Cells, orijinal yazı tipiyle aynı aileye sahip evrensel yazı tipini kullanır,<br/> varsayılan değer boştur.|
| [worksheet_scalable](/cells/tr/python-net/aspose.cells/htmlsaveoptions/worksheet_scalable) |Dosyayı html'ye kaydederken çalışma sayfası yakınlaştırma düzeyi yoluyla html'nin yakınlaştırılıp uzaklaştırılmadığını gösterir, varsayılan değer yanlıştır.|
| [is_export_comments](/cells/tr/python-net/aspose.cells/htmlsaveoptions/is_export_comments) | Dosyayı html'ye kaydederken yorumların dışa aktarılıp aktarılmadığını gösterir, varsayılan değer yanlıştır.|
| [export_comments_type](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_comments_type) | Yorumları html dosyalarına aktarma türünü temsil eder.|
| [disable_downlevel_revealed_comments](/cells/tr/python-net/aspose.cells/htmlsaveoptions/disable_downlevel_revealed_comments) | Dosyayı html'ye dışa aktarırken Alt Düzeyde ortaya çıkan koşullu yorumları devre dışı bırakıp bırakmadığınızı belirtir, varsayılan değer yanlıştır.|
| [is_exp_image_to_temp_dir](/cells/tr/python-net/aspose.cells/htmlsaveoptions/is_exp_image_to_temp_dir) | Görüntü dosyalarının geçici dizine aktarılıp aktarılmadığını gösterir.<br/> Yalnızca html akışına kaydetmek için.|
| [image_scalable](/cells/tr/python-net/aspose.cells/htmlsaveoptions/image_scalable) | Görüntü genişliğini açıklamak için ölçeklenebilir birim kullanılıp kullanılmadığını gösterir<br/>sütun genişliğini açıklamak için ölçeklenebilir birim kullanıldığında.<br/> Varsayılan değer doğrudur.|
| [width_scalable](/cells/tr/python-net/aspose.cells/htmlsaveoptions/width_scalable) | Dosyayı html'ye dışa aktarırken sütun genişliğini açıklamak için ölçeklenebilir birim kullanılıp kullanılmadığını gösterir.<br/> Varsayılan değer yanlıştır.|
| [export_single_tab](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_single_tab) | Dosyada yalnızca bir çalışma sayfası olduğunda tek sekmenin dışa aktarılıp aktarılmadığını gösterir.<br/> Varsayılan değer yanlıştır.|
| [export_images_as_base64](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_images_as_base64) | Resimlerin Base64 formatında HTML, MHTML veya EPUB'a kaydedilip kaydedilmeyeceğini belirtir.|
| [export_active_worksheet_only](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_active_worksheet_only) | Tüm çalışma kitabının html dosyasına aktarılıp aktarılmadığını gösterir.|
| [export_print_area_only](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_print_area_only) | Yalnızca yazdırma alanının html dosyasına aktarılıp aktarılmadığını gösterir. Varsayılan değer yanlıştır.|
| [export_area](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_area) | Geçerli etkin Çalışma Sayfasının dışa aktarılan CellArea'sını Alır veya Ayarlar.<br/>Bu özniteliği ayarlarsanız, geçerli etkin Çalışma Sayfasının yazdırma alanı çıkarılacaktır.<br/> Dosya html'ye kaydedilirken yalnızca belirtilen alan dışa aktarılacaktır.|
| [parse_html_tag_in_cell](/cells/tr/python-net/aspose.cells/htmlsaveoptions/parse_html_tag_in_cell) | Html etiketini hücrede, hücre değeri olarak veya html etiketi gibi ayrıştırın, varsayılan değer doğrudur|
| [html_cross_string_type](/cells/tr/python-net/aspose.cells/htmlsaveoptions/html_cross_string_type) | Bir Excel dosyasını html biçiminde kaydederken, hücreler arası bir dizenin MS Excel ile aynı şekilde görüntülenip görüntülenmeyeceğini belirtir.<br/>Varsayılan olarak değer Varsayılan'dır, dolayısıyla hücreler arası dizeler için Aspose.Cells tarafından oluşturulan html dosyaları ile MS Excel arasında çok az fark vardır.<br/>Ancak büyük html dosyaları oluşturma performansı, değeri Çapraz olarak ayarlamak, Varsayılan veya Fit2Cell olarak ayarlamaktan birkaç kat daha hızlı olacaktır.|
| [hidden_col_display_type](/cells/tr/python-net/aspose.cells/htmlsaveoptions/hidden_col_display_type) | Excel'de gizli sütun (bu sütunun genişliği 0'dır), bunu html biçiminde kaydetmeden önce,<br/>HtmlHiddenColDisplayType "Kaldır" ise, gizli sütunun çıkışı olmaz,<br/> değer "Gizli" ise, sütun çıktısı alınır, ancak gizlidir, varsayılan değer "Gizli" olur|
| [hidden_row_display_type](/cells/tr/python-net/aspose.cells/htmlsaveoptions/hidden_row_display_type) | Excel'de gizli satır (bu satırın yüksekliği 0'dır), bunu html biçiminde kaydetmeden önce,<br/>HtmlHiddenRowDisplayType "Kaldır" ise, gizli satır çıkarılmaz,<br/> değer "Gizli" ise, satır çıkar, ancak gizlenir, varsayılan değer "Gizli" olur|
| [encoding](/cells/tr/python-net/aspose.cells/htmlsaveoptions/encoding) | Ayarlanmamışsa varsayılan kodlama türü olarak Encoding.UTF8'i kullanın.|
| [export_object_listener](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_object_listener) | Nesneleri dışa aktarmak için ExportObjectListener öğesini alır veya ayarlar.|
| [file_path_provider](/cells/tr/python-net/aspose.cells/htmlsaveoptions/file_path_provider) | Çalışma Sayfasını html'ye ayrı olarak dışa aktarmak için IFilePathProvider'ı alır veya ayarlar.|
| [stream_provider](/cells/tr/python-net/aspose.cells/htmlsaveoptions/stream_provider) | Nesneleri dışa aktarmak için IStreamProvider öğesini alır veya ayarlar.|
| [image_options](/cells/tr/python-net/aspose.cells/htmlsaveoptions/image_options) | Dışa aktarmadan önce ImageOrPrintOptions nesnesini alın|
| [save_as_single_file](/cells/tr/python-net/aspose.cells/htmlsaveoptions/save_as_single_file) | Html'nin tek dosya olarak kaydedilip kaydedilmediğini gösterir.<br/> Varsayılan değer yanlıştır.|
| [show_all_sheets](/cells/tr/python-net/aspose.cells/htmlsaveoptions/show_all_sheets) | Tek bir html dosyası olarak kaydederken tüm sayfaların gösterilip gösterilmediğini belirtir.|
| [export_page_headers](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_page_headers) | Sayfa başlıklarının dışa aktarılıp aktarılmadığını gösterir.|
| [export_page_footers](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_page_footers) | Sayfa başlıklarının dışa aktarılıp aktarılmadığını gösterir.|
| [export_hidden_worksheet](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_hidden_worksheet) |Gizli çalışma sayfası içeriğinin dışa aktarılıp aktarılmadığını belirtir. Varsayılan değer doğrudur.|
| [presentation_preference](/cells/tr/python-net/aspose.cells/htmlsaveoptions/presentation_preference) | Sunum tercihinin html mi yoksa mht dosyası mı olduğunu belirtmek.<br/>Varsayılan değer yanlıştır.<br/> Daha güzel bir sunum elde etmek istiyorsanız, lütfen değeri true olarak ayarlayın.|
| [cell_css_prefix](/cells/tr/python-net/aspose.cells/htmlsaveoptions/cell_css_prefix) | Css adının önekini alır ve ayarlar, varsayılan değer "" dir.|
| [table_css_id](/cells/tr/python-net/aspose.cells/htmlsaveoptions/table_css_id) |css adının tr,col,td vb. gibi ön ekini alır ve ayarlar, bunlar tablo öğesinde bulunur<br/> belirli TableCssId özniteliğine sahip olan. Varsayılan değer "" şeklindedir.|
| [is_full_path_link](/cells/tr/python-net/aspose.cells/htmlsaveoptions/is_full_path_link) | Sheet00x.htm,filelist.xml ve tabstrip.htm'de tam yol bağlantısının kullanılıp kullanılmadığını belirtir.<br/> Varsayılan değer yanlıştır.|
| [export_worksheet_css_separately](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_worksheet_css_separately) | Çalışma sayfası css'sinin ayrı olarak dışa aktarılıp aktarılmadığını belirtir. Varsayılan değer yanlıştır.|
| [export_similar_border_style](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_similar_border_style) | Kenarlık stili tarayıcılar tarafından desteklenmediğinde benzer kenarlık stilinin dışa aktarılıp aktarılmadığını gösterir.<br/>Html veya mht dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.<br/> Varsayılan değer yanlıştır.|
| [merge_empty_td_forcely](/cells/tr/python-net/aspose.cells/htmlsaveoptions/merge_empty_td_forcely) | Dosyayı html'ye dışa aktarırken boş TD öğesinin zorla birleştirilip birleştirilmediğini gösterir.<br/> Değer true olarak ayarlandıktan sonra html dosyasının boyutu önemli ölçüde azaltılacaktır. Varsayılan değer yanlıştır.<br/> Html dosyasını excel'e aktarmak veya dosyayı html'ye kaydederken mükemmel ızgara çizgilerini dışa aktarmak istiyorsanız,<br/> lütfen varsayılan değeri koruyun.|
| [export_cell_coordinate](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_cell_coordinate) | Dosyayı html'ye kaydederken boş olmayan hücrelerin excel koordinatlarının dışa aktarılıp aktarılmadığını gösterir. Varsayılan değer yanlıştır.<br/> Çıktı html'sini excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.|
| [export_extra_headings](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_extra_headings) | Metin uzunluğu maksimum görüntüleme sütunundan daha uzun olduğunda fazladan başlıkların dışa aktarılıp aktarılmayacağını gösterir.<br/> Varsayılan değer yanlıştır. Html dosyasını excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.|
| [export_headings](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_headings) | HTML dosyasına kaydederken sayfanın satır ve sütun başlıklarının dışa aktarılıp aktarılmayacağını belirtir.|
| [export_row_column_headings](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_row_column_headings) | HTML dosyasına kaydederken sayfanın satır ve sütun başlıklarının dışa aktarılıp aktarılmayacağını belirtir.|
| [export_formula](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_formula) | Dosyayı html'ye kaydederken formülün dışa aktarılıp aktarılmadığını gösterir. Varsayılan değer doğrudur.<br/> Çıktı html'sini excel'e aktarmak istiyorsanız, lütfen varsayılan değeri koruyun.|
| [add_tooltip_text](/cells/tr/python-net/aspose.cells/htmlsaveoptions/add_tooltip_text) |Veriler tam olarak görüntülenemediğinde araç ipucu metni eklenip eklenmeyeceğini belirtir.<br/> Varsayılan değer yanlıştır.|
| [export_grid_lines](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_grid_lines) | Kılavuz çizgilerinin dışa aktarılıp aktarılmadığını belirtir. Varsayılan değer yanlıştır.|
| [export_bogus_row_data](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_bogus_row_data) | Sahte alt satır verilerinin dışa aktarılıp aktarılmadığını belirtir. Varsayılan değer true'dur. Eğer html veya mht dosyasını içe aktarmak istiyorsanız<br/> excel için lütfen varsayılan değeri koruyun.|
| [exclude_unused_styles](/cells/tr/python-net/aspose.cells/htmlsaveoptions/exclude_unused_styles) | Kullanılmayan stillerin hariç tutulup tutulmadığını belirtir.<br/>Oluşturulan html dosyaları için, kullanılmayan stilleri hariç tutmak, dosya boyutunu küçültebilir<br/>görsel efektleri etkilemeden. Dolayısıyla, bu özelliğin varsayılan değeri doğrudur.<br/>Kullanıcının oluşturulan html için çalışma kitabındaki tüm stilleri tutması gerekiyorsa (kullanıcının kullandığı senaryo gibi)<br/> çalışma kitabını daha sonra oluşturulan html'den geri yüklemesi gerekiyor), lütfen bu özelliği yanlış olarak ayarlayın.|
| [export_document_properties](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_document_properties) | Belge özelliklerinin dışa aktarılıp aktarılmadığını belirtir. Varsayılan değer true'dur. İçe aktarmak istiyorsanız<br/> html veya mht dosyasını excel'e gönderirken, lütfen varsayılan değeri koruyun.|
| [export_worksheet_properties](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_worksheet_properties) | Çalışma sayfası özelliklerinin dışa aktarılıp aktarılmadığını belirtir.Varsayılan değer true'dur.İçe aktarmak istiyorsanız<br/> html veya mht dosyasını excel'e gönderirken, lütfen varsayılan değeri koruyun.|
| [export_workbook_properties](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_workbook_properties) | Çalışma kitabı özelliklerinin dışa aktarılıp aktarılmadığını belirtir. Varsayılan değer true'dur. Almak istiyorsanız<br/> html veya mht dosyasını excel'e gönderirken, lütfen varsayılan değeri koruyun.|
| [export_frame_scripts_and_properties](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_frame_scripts_and_properties) | Çerçeve betiklerinin ve belge özelliklerinin dışa aktarılıp aktarılmadığını belirtir. Varsayılan değer true'dur. Eğer html veya mht dosyasını içe aktarmak istiyorsanız<br/> excel için lütfen varsayılan değeri koruyun.|
| [export_data_options](/cells/tr/python-net/aspose.cells/htmlsaveoptions/export_data_options) | Html dosyası verilerini dışa aktarma kuralını belirtir. Varsayılan değer Tümüdür.|
| [link_target_type](/cells/tr/python-net/aspose.cells/htmlsaveoptions/link_target_type) | Hedef öznitelik türünün belirtilmesi<a> link,Varsayılan değer HtmlLinkTargetType.Parent'tir.|



###  Ayrıca bakınız
* modül [aspose.cells](..)
* sınıf [HtmlSaveOptions](/cells/tr/python-net/aspose.cells/htmlsaveoptions)
* sınıf [SaveOptions](/cells/tr/python-net/aspose.cells/saveoptions)
