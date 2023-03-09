---
title: create_safe_sheet_name yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 90
url: /tr/python-net/aspose.cells/cellshelper/create_safe_sheet_name/
is_root: false
---
##  create_safe_sheet_name(name_proposal) {#str}
Verilen sayfa adını kontrol eder ve gerektiğinde geçerli bir tane oluşturur.
Verilen sayfa adı excel sayfa adı kurallarına uygunsa iade edin.
Aksi takdirde, uzunluk sınırı aşarsa dize kesilir
ve geçersiz karakterler '' ile değiştirilecek, ardından yeniden oluşturulmuş dize değerini döndürecektir.


###  İadeler




```python
def create_safe_sheet_name(self, name_proposal):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| name_proposal | str | kullanılacak sayfa adı|


##  create_safe_sheet_name(name_proposal, replace_char) {#str-char}
Verilen sayfa adını kontrol eder ve gerektiğinde geçerli bir tane oluşturur.
Verilen sayfa adı excel sayfa adı kurallarına uygunsa iade edin.
Aksi takdirde, uzunluk sınırı aşarsa dize kesilir
ve geçersiz karakterler verilen karakterle değiştirilecek, ardından yeniden oluşturulmuş dize değerini döndürecektir.


###  İadeler




```python
def create_safe_sheet_name(self, name_proposal, replace_char):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| name_proposal | str | kullanılacak sayfa adı|
| replace_char | char | verilen sayfa adındaki geçersiz karakterleri değiştirmek için kullanılacak karakter|



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [CellsHelper](/cells/tr/python-net/aspose.cells/cellshelper)
