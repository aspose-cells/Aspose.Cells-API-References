---
title: to_printer yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 50
url: /tr/python-net/aspose.cells.rendering/sheetrender/to_printer/
is_root: false
---
##  to_printer(printer_name) {#str}
Çalışma sayfasını Yazıcıya işle



```python
def to_printer(self, printer_name):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| printer_name | str | yazıcının adı , örneğin: "Microsoft Office Document Image Writer"|


##  to_printer(printer_settings) {#aspose.pydrawing.printing.PrinterSettings}
Çalışma sayfasını Yazıcıya işle



```python
def to_printer(self, printer_settings):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| printer_settings | aspose.pydrawing.printing.PrinterSettings | yazıcının ayarları, örneğin YazıcıAdı, Dubleks|


##  to_printer(printer_name, job_name) {#str-str}
Çalışma sayfasını Yazıcıya işle



```python
def to_printer(self, printer_name, job_name):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| printer_name | str | yazıcının adı , örneğin: "Microsoft Office Document Image Writer"|
| job_name | str | yazdırma işi adını ayarla|


##  to_printer(printer_settings, job_name) {#aspose.pydrawing.printing.PrinterSettings-str}
Çalışma sayfasını Yazıcıya işle



```python
def to_printer(self, printer_settings, job_name):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| printer_settings | aspose.pydrawing.printing.PrinterSettings | yazıcının ayarları, örneğin YazıcıAdı, Dubleks|
| job_name | str | yazdırma işi adını ayarla|


##  to_printer(printer_name, print_page_index, print_page_count) {#str-int-int}
Çalışma sayfasını Yazıcıya işle



```python
def to_printer(self, printer_name, print_page_index, print_page_count):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| printer_name | str | yazıcının adı , örneğin: "Microsoft Office Document Image Writer"|
| print_page_index | int | yazdırılacak ilk sayfanın 0 tabanlı dizini, Aralık [0, SheetRender.PageCount-1] olmalıdır|
| print_page_count | int | yazdırılacak sayfa sayısı sıfırdan büyük olmalıdır|
###  Notlar

NOT: Bu yöntem artık kullanılmıyor.
Bunun yerine, ilk sayfayı ve yazdırılacak sayfa sayısını ayarlamak için lütfen ToPrinter(string PrinterName) ve ImageOrPrintOptions.PageIndex, PageCount'u kullanın.
 Bu mülk, Aralık 2021'den bu yana 12 ay sonra kaldırılacaktır.
Aspose yaşamış olabileceğiniz rahatsızlıktan dolayı özür diler.


###  Ayrıca bakınız
* modül [aspose.cells.rendering](../../)
* sınıf [SheetRender](/cells/tr/python-net/aspose.cells.rendering/sheetrender)
