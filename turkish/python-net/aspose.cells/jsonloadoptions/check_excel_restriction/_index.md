---
title: check_excel_restriction mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 70
url: /tr/python-net/aspose.cells/jsonloadoptions/check_excel_restriction/
is_root: false
---
##  check_excel_restriction mülk

Kullanıcı hücrelerle ilgili nesneleri değiştirdiğinde excel dosyasının kısıtlamasının kontrol edilip edilmeyeceği.
Örneğin, excel 32K'dan daha uzun bir dizi değeri girilmesine izin vermez.
Cell.PutValue(string) gibi 32K'dan uzun bir değer girdiğinizde, bu özellik doğruysa, bir İstisna alırsınız.
Bu özellik yanlışsa, giriş dizesi değerinizi hücrenin değeri olarak kabul edeceğiz, böylece daha sonra
CSV gibi diğer dosya formatları için tam dizi değerinin çıktısını alabilirsiniz.
Ancak excel dosya formatı için geçersiz olan bir değer belirlediyseniz,
çalışma kitabını daha sonra excel dosya formatında kaydetmemelisiniz. Aksi halde oluşturulan excel dosyasında beklenmeyen bir hata olabilir.
###  Tanım:
```python
@property
def check_excel_restriction(self):
    ...
@check_excel_restriction.setter
def check_excel_restriction(self, value):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [JsonLoadOptions](/cells/tr/python-net/aspose.cells/jsonloadoptions)
