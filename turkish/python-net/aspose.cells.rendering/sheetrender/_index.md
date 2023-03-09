---
title: SheetRender sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 100
url: /tr/python-net/aspose.cells.rendering/sheetrender/
is_root: false
---
##  SheetRender sınıfı
Çalışma sayfasını (BMP, PNG, JPEG, TIFF..) gibi çeşitli görüntülere işleyebilen bir çalışma sayfası oluşturmayı temsil eder.
Bu sınıfın yapıcısı, sayfa düzeni, hücre stili değiştirildikten sonra kullanılmalıdır.



SheetRender türü aşağıdaki üyeleri gösterir:

###  İnşaatçılar
| Yapıcı| Tanım|
| :- | :- |
| [SheetRender(worksheet, options)](/cells/tr/python-net/aspose.cells.rendering/sheetrender/__init__/#Worksheet-ImageOrPrintOptions) | SheetRender yapısı, param olarak çalışma sayfası ve ImageOrPrintOptions'a ihtiyaç duyar|


###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [page_count](/cells/tr/python-net/aspose.cells.rendering/sheetrender/page_count) | Geçerli çalışma sayfasının toplam sayfa sayısını alır.|
| [page_scale](/cells/tr/python-net/aspose.cells.rendering/sheetrender/page_scale) | Sayfanın hesaplanan sayfa ölçeğini alır.<br/> [PageSetup.zoom](/cells/tr/python-net/aspose.cells/pagesetup#zoom) ayarlanmışsa ayarlanan ölçeği döndürür.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [to_image(page_index, file_name)](/cells/tr/python-net/aspose.cells.rendering/sheetrender/to_image/#int-str) | Belirli sayfaları bir dosyaya dönüştürün.|
| [to_image(page_index, stream)](/cells/tr/python-net/aspose.cells.rendering/sheetrender/to_image/#int-io.RawIOBase) | Belirli sayfaları bir akışa dönüştürün.|
| [to_tiff(stream)](/cells/tr/python-net/aspose.cells.rendering/sheetrender/to_tiff/#io.RawIOBase) | Akış için tüm çalışma sayfasını Tiff Görüntüsü olarak işleyin.|
| [to_tiff(filename)](/cells/tr/python-net/aspose.cells.rendering/sheetrender/to_tiff/#str) | Tüm çalışma sayfasını bir dosyaya Tiff Görüntüsü olarak işleyin.|
| [to_printer(printer_name)](/cells/tr/python-net/aspose.cells.rendering/sheetrender/to_printer/#str) | Çalışma sayfasını yazıcıya işle|
| [to_printer(printer_name, job_name)](/cells/tr/python-net/aspose.cells.rendering/sheetrender/to_printer/#str-str) | Çalışma sayfasını yazıcıya işle|
| [to_printer(printer_settings)](/cells/tr/python-net/aspose.cells.rendering/sheetrender/to_printer/#aspose.pydrawing.printing.PrinterSettings) | Çalışma sayfasını yazıcıya işle|
| [to_printer(printer_settings, job_name)](/cells/tr/python-net/aspose.cells.rendering/sheetrender/to_printer/#aspose.pydrawing.printing.PrinterSettings-str) | Çalışma sayfasını yazıcıya işle|
| [to_printer(printer_name, print_page_index, print_page_count)](/cells/tr/python-net/aspose.cells.rendering/sheetrender/to_printer/#str-int-int) | Çalışma sayfasını yazıcıya işle|
| [get_page_size_inch(page_index)](/cells/tr/python-net/aspose.cells.rendering/sheetrender/get_page_size_inch/#int) |Çıktı görüntüsünün inç cinsinden sayfa boyutunu alın.|
| [custom_print(next_page_after_print, print_page_event_args)](/cells/tr/python-net/aspose.cells.rendering/sheetrender/custom_print/#bool-aspose.pydrawing.printing.PrintPageEventArgs) | İstemci, bu işlevi kullanarak her sayfayı yazdırırken yazıcının sayfa ayarını kontrol edebilir.|



###  Ayrıca bakınız
* modül [aspose.cells.rendering](..)
