---
title: ImageOrPrintOptions sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 40
url: /tr/python-net/aspose.cells.rendering/imageorprintoptions/
is_root: false
---
##  ImageOrPrintOptions sınıfı
Çalışma sayfasını görüntülere dönüştürürken, çalışma sayfasını yazdırırken veya tabloyu görüntüye dönüştürürken seçenekleri belirlemeye izin verir.



ImageOrPrintOptions türü aşağıdaki üyeleri gösterir:

###  İnşaatçılar
| Yapıcı| Tanım|
| :- | :- |
| [ImageOrPrintOptions()](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/__init__/#) | ImageOrPrintOptions'ın yeni bir örneğini oluşturur|


###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [save_format](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/save_format) | Çıktı dosyası biçim türünü alır veya ayarlar<br/> Destek Tiff/XPS|
| [print_with_status_dialog](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/print_with_status_dialog) | PrintWithStatusDialog = true ise, geçerli yazdırma durumunu gösteren bir iletişim kutusu olacaktır.<br/> aksi halde böyle bir iletişim kutusu gösterilmez.|
| [horizontal_resolution](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/horizontal_resolution) | Oluşturulan görüntülerin yatay çözünürlüğünü inç başına nokta cinsinden alır veya ayarlar.<br/> Emf biçimli görüntüler dışında görüntü oluşturma yöntemini uygular.|
| [vertical_resolution](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/vertical_resolution) | Oluşturulan görüntülerin dikey çözünürlüğünü inç başına nokta cinsinden alır veya ayarlar.<br/> Emf biçimli görüntü dışında görüntü oluşturma yöntemini uygular.|
| [tiff_compression](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/tiff_compression) | Yalnızca sayfaları `Tiff` biçiminde kaydederken uygulanacak sıkıştırma türünü alır veya ayarlar.|
| [tiff_color_depth](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/tiff_color_depth) | Yalnızca sayfaları `Tiff` biçiminde kaydederken uygulanacak bit derinliğini alır veya ayarlar.|
| [printing_page](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/printing_page) | Hangi sayfaların yazdırılmayacağını belirtir.|
| [quality](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/quality) | Oluşturulan görüntülerin kalitesini belirleyen bir değer alır veya ayarlar<br/>yalnızca sayfaları `Jpeg` biçiminde kaydederken uygulanacak.|
| [image_type](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/image_type) | Oluşturulan görüntülerin biçimini alır veya ayarlar.<br/> varsayılan değer: PNG.|
| [is_cell_auto_fit](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/is_cell_auto_fit) | Hücrelerin genişliğinin ve yüksekliğinin hücre değerine göre otomatik olarak sığdırılıp uydurulmadığını gösterir.<br/> Varsayılan değer yanlıştır.|
| [one_page_per_sheet](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/one_page_per_sheet) | OnePagePerSheet true ise, sonuçta bir sayfanın tüm içeriği yalnızca bir sayfaya çıkar.<br/> pagesetup'ın kağıt boyutu geçersiz olacak ve pagesetup'ın diğer ayarları geçersiz olacaktır.<br/> yine de geçerli olacaktır.|
| [all_columns_in_one_page_per_sheet](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/all_columns_in_one_page_per_sheet) | AllColumnsInOnePagePerSheet true olursa, bir sayfanın tüm sütun içeriği sonuçta yalnızca bir sayfaya çıkar.<br/> pagesetup'ın kağıt boyutunun genişliği geçersiz olacaktır ve pagesetup'ın diğer ayarları geçersiz olacaktır.<br/> yine de geçerli olacaktır.|
| [draw_object_event_handler](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/draw_object_event_handler) | İşleme sırasında DrawObject ve Bound'u almak için bu arabirimi uygular.|
| [chart_image_type](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/chart_image_type) | Dönüştürürken grafik görüntü tipini belirtin.<br/> varsayılan değer: PNG.|
| [embeded_image_name_in_svg](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/embeded_image_name_in_svg) | Gömülü görüntünün dosya adını svg'de belirtin.<br/> Bu, "c:\\xpsEmbedded" gibi bir dizine sahip tam yol olmalıdır.|
| [svg_fit_to_view_port](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/svg_fit_to_view_port) | bu özellik doğruysa, oluşturulan svg bağlantı noktasını görüntülemeye sığar.|
| [only_area](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/only_area) | Bu özellik true ise, bir Alan çıktısı alınır ve hiçbir ölçek etkili olmaz.|
| [text_rendering_hint](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/text_rendering_hint) | Metin oluşturma kalitesini belirtir.<br/> Varsayılan değer TextRenderingHint'tir.SystemDefault|
| [smoothing_mode](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/smoothing_mode) | Çizgilere, eğrilere ve dolgulu alanların kenarlarına yumuşatma (kenar yumuşatma) uygulanıp uygulanmayacağını belirtir.<br/> Varsayılan değer SmoothingMode.None şeklindedir.|
| [transparent](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/transparent) | Oluşturulan görüntünün arka planının saydam olup olmayacağını belirtir.|
| [pixel_format](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/pixel_format) |Oluşturulan görüntüler için piksel biçimini alır veya ayarlar.|
| [warning_callback](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/warning_callback) | Uyarı geri aramalarını alır veya ayarlar.|
| [page_saving_callback](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/page_saving_callback) | Sayfa kaydetme işleminin ilerleyişini kontrol edin/gösterin.|
| [is_font_substitution_char_granularity](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/is_font_substitution_char_granularity) | Yalnızca hücre yazı tipi uyumlu olmadığında karakter yazı tipinin değiştirilip değiştirilmeyeceğini belirtir.|
| [page_index](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/page_index) | Kaydedilecek ilk sayfanın 0 tabanlı dizinini alır veya ayarlar.|
| [page_count](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/page_count) | Kaydedilecek sayfa sayısını alır veya ayarlar.|
| [is_optimized](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/is_optimized) | Çıkış öğelerinin optimize edilip edilmeyeceğini gösterir.|
| [default_font](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/default_font) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipiyle ayarlanmadığında,<br/>Pdf, görüntüde blok olarak görünebilirler.<br/>Bu karakterleri göstermek için MingLiu veya MS Gothic gibi bir Varsayılan Yazı Tipi ayarlayın.<br/> Bu özellik ayarlanmazsa, Aspose.Cells, bu unicode karakterleri göstermek için sistem varsayılan yazı tipini kullanır.|
| [check_workbook_default_font](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/check_workbook_default_font) | Excel'deki karakterler Unicode olduğunda ve hücre stilinde doğru yazı tipiyle ayarlanmadığında,<br/>Pdf, görüntüde blok olarak görünebilirler.<br/> Önce bu karakterleri göstermek için çalışma kitabının varsayılan yazı tipini kullanmayı denemek için bunu true olarak ayarlayın.|
| [output_blank_page_when_nothing_to_print](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/output_blank_page_when_nothing_to_print) | Yazdırılacak bir şey olmadığında boş bir sayfa çıktısı alınıp alınmayacağını belirtir.|
| [gridline_type](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/gridline_type) | Kılavuz çizgisi türünü alır veya ayarlar.|
| [text_cross_type](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/text_cross_type) | Metin genişliği hücre genişliğinden büyük olduğunda görüntülenen metin türünü alır veya ayarlar.|
| [emf_type](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/emf_type) | Meta dosyasının biçimini belirten bir EmfType alır veya ayarlar.<br/> Varsayılan değer EmfPlusDual'dır.|
| [default_edit_language](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/default_edit_language) | Varsayılan düzenleme dilini alır veya ayarlar.|
| [sheet_set](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/sheet_set) |İşlenecek sayfaları alır veya ayarlar. Varsayılan, çalışma kitabındaki tüm görünür sayfalardır: [SheetSet.visible](/cells/tr/python-net/aspose.cells.rendering/sheetset#visible).|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [set_desired_size(desired_width, desired_height)](/cells/tr/python-net/aspose.cells.rendering/imageorprintoptions/set_desired_size/#int-int) | Görüntünün istenen genişliğini ve yüksekliğini ayarlar.|



###  örnekler

```python
from aspose.cells import Workbook
from aspose.cells.drawing import ImageType
from aspose.cells.rendering import ImageOrPrintOptions

# Set Image Or Print Options
options = ImageOrPrintOptions()
# Set output image format
options.image_type = ImageType.PNG
# Set Horizontal resolution
options.horizontal_resolution = 300
# Set Vertical Resolution
options.vertical_resolution = 300
# Instantiate Workbook
book = Workbook("test.xls")
# Save chart as Image using ImageOrPrint Options
book.worksheets[0].charts[0].to_image("chart.png", options)

```

###  Ayrıca bakınız
* modül [aspose.cells.rendering](..)
