---
title: Workbook yapıcı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 10
url: /tr/python-net/aspose.cells/workbook/__init__/
is_root: false
---
##  Workbook() {#}
[Workbook](/cells/tr/python-net/aspose.cells/workbook) sınıfının yeni bir örneğini başlatır.



```python
def __init__(self):
    ...
```


###  Notlar

Varsayılan dosya biçimi türü Xlsx'tir. Başka formatta dosya türü oluşturmak için lütfen Workbook(FileFormatType) kullanın.
###  Örnek


Aşağıdaki kod, sınıfın yeni bir örneğini oluşturmak ve başlatmak için Workbook yapıcısının nasıl kullanılacağını gösterir.

```python
from aspose.cells import Workbook

workbook = Workbook()

```


##  Workbook(file_format_type) {#FileFormatType}
[Workbook](/cells/tr/python-net/aspose.cells/workbook) sınıfının yeni bir örneğini başlatır.



```python
def __init__(self, file_format_type):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| file_format_type | [FileFormatType](/cells/tr/python-net/aspose.cells/fileformattype) | Yeni dosya formatı.|
###  Notlar

Varsayılan dosya biçimi türü Excel97To2003'tür.
###  Örnek


Aşağıdaki kod, sınıfın yeni bir örneğini oluşturmak ve başlatmak için Workbook yapıcısının nasıl kullanılacağını gösterir.

```python
from aspose.cells import FileFormatType, Workbook

workbook = Workbook(FileFormatType.XLSX)

```


##  Workbook(file) {#str}
[Workbook](/cells/tr/python-net/aspose.cells/workbook) sınıfının yeni bir örneğini başlatır ve bir dosya açar.



```python
def __init__(self, file):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| file | str | Dosya adı.|


##  Workbook(stream) {#io.RawIOBase}
[Workbook](/cells/tr/python-net/aspose.cells/workbook) sınıfının yeni bir örneğini başlatır ve bir akış açar.



```python
def __init__(self, stream):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| stream | io.RawIOBase | Akış.|


##  Workbook(file, load_options) {#str-LoadOptions}
[Workbook](/cells/tr/python-net/aspose.cells/workbook) sınıfının yeni bir örneğini başlatır ve bir dosya açar.



```python
def __init__(self, file, load_options):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| file | str | Dosya adı.|
| load_options | [LoadOptions](/cells/tr/python-net/aspose.cells/loadoptions) | yükleme seçenekleri|


##  Workbook(stream, load_options) {#io.RawIOBase-LoadOptions}
[Workbook](/cells/tr/python-net/aspose.cells/workbook) sınıfının ve açık akışın yeni bir örneğini başlatır.



```python
def __init__(self, stream, load_options):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| stream | io.RawIOBase | Akış.|
| load_options | [LoadOptions](/cells/tr/python-net/aspose.cells/loadoptions) | yükleme seçenekleri|



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Workbook](/cells/tr/python-net/aspose.cells/workbook)
