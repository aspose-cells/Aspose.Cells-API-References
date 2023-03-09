---
title: check_font_compatibility mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 50
url: /tr/python-net/aspose.cells/pptxsaveoptions/check_font_compatibility/
is_root: false
---
##  check_font_compatibility mülk

Metindeki her karakter için yazı tipi uyumluluğunun kontrol edilip edilmeyeceğini belirtir.

###  Notlar

Varsayılan değer doğrudur.
Bu özelliği devre dışı bırakmak daha iyi performans sağlayabilir.
Ancak varsayılan veya belirtilen metin/karakter yazı tipi onu oluşturmak için kullanılamıyorsa,
oluşturulan pdf'de okunamayan karakterler (blok gibi) oluşabilir.
Böyle bir durum için kullanıcı bu özelliği true olarak tutmalıdır, böylece
bunun yerine metni oluşturmak için alternatif yazı tipi aranabilir ve kullanılabilir;
###  Tanım:
```python
@property
def check_font_compatibility(self):
    ...
@check_font_compatibility.setter
def check_font_compatibility(self, value):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [PptxSaveOptions](/cells/tr/python-net/aspose.cells/pptxsaveoptions)
