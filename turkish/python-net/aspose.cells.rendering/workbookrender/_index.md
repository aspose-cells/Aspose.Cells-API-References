---
title: WorkbookRender sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 130
url: /tr/python-net/aspose.cells.rendering/workbookrender/
is_root: false
---
##  WorkbookRender sınıf
 Bir Çalışma Kitabı işlemesini temsil eder.
Bu sınıfın yapıcısı, sayfa düzeni, hücre stili değiştirildikten sonra kullanılmalıdır.



WorkbookRender türü aşağıdaki üyeleri gösterir:

###  İnşaatçılar
| Yapıcı| Tanım|
| :- | :- |
| [WorkbookRender(workbook, options)](/cells/tr/python-net/aspose.cells.rendering/workbookrender/__init__/#Workbook-ImageOrPrintOptions) | WorkbookRender'ın yapısı|


###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [page_count](/cells/tr/python-net/aspose.cells.rendering/workbookrender/page_count) | Çalışma kitabının toplam sayfa sayısını alır.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [to_image(stream)](/cells/tr/python-net/aspose.cells.rendering/workbookrender/to_image/#io.RawIOBase) | Akış için tüm çalışma kitabını Tiff Görüntüsü olarak işleyin.|
| [to_image(filename)](/cells/tr/python-net/aspose.cells.rendering/workbookrender/to_image/#str) | Tüm çalışma kitabını bir dosyaya Tiff Görüntüsü olarak işleyin.|
| [to_image(page_index, file_name)](/cells/tr/python-net/aspose.cells.rendering/workbookrender/to_image/#int-str) | Belirli bir sayfayı bir dosyaya dönüştürün.|
| [to_image(page_index, stream)](/cells/tr/python-net/aspose.cells.rendering/workbookrender/to_image/#int-io.RawIOBase) | Belirli bir sayfayı bir akışa dönüştürün.|
| [to_printer(printer_name)](/cells/tr/python-net/aspose.cells.rendering/workbookrender/to_printer/#str) | Çalışma kitabını Yazıcıya işle|
| [to_printer(printer_name, job_name)](/cells/tr/python-net/aspose.cells.rendering/workbookrender/to_printer/#str-str) | Çalışma kitabını Yazıcıya işle|
| [to_printer(printer_settings)](/cells/tr/python-net/aspose.cells.rendering/workbookrender/to_printer/#aspose.pydrawing.printing.PrinterSettings) | Çalışma kitabını Yazıcıya işle|
| [to_printer(printer_settings, job_name)](/cells/tr/python-net/aspose.cells.rendering/workbookrender/to_printer/#aspose.pydrawing.printing.PrinterSettings-str) | Çalışma kitabını Yazıcıya işle|
| [to_printer(printer_name, print_page_index, print_page_count)](/cells/tr/python-net/aspose.cells.rendering/workbookrender/to_printer/#str-int-int) | Çalışma kitabını Yazıcıya işle|
| [get_page_size_inch(page_index)](/cells/tr/python-net/aspose.cells.rendering/workbookrender/get_page_size_inch/#int) | Çıktı görüntüsünün inç cinsinden sayfa boyutunu alın.|
| [custom_print(next_page_after_print, print_page_event_args)](/cells/tr/python-net/aspose.cells.rendering/workbookrender/custom_print/#bool-aspose.pydrawing.printing.PrintPageEventArgs) | İstemci, bu işlevi kullanarak her sayfayı yazdırırken yazıcının sayfa ayarını kontrol edebilir.|



###  Notlar



###  Ayrıca bakınız
* modül [aspose.cells.rendering](..)
