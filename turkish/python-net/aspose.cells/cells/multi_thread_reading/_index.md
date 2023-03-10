---
title: multi_thread_reading mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 1200
url: /tr/python-net/aspose.cells/cells/multi_thread_reading/
is_root: false
---
##  multi_thread_reading mülk

Hücre veri modelinin Multi-Thread okumayı desteklemesi gerekip gerekmediğini alır veya ayarlar.
Bu özelliğin varsayılan değeri yanlıştır.

###  Notlar

Bu koleksiyondaki Row/Cell nesnelerini aynı anda okumak için birden çok iş parçacığı varsa,
bu özellik true olarak ayarlanmalıdır, aksi takdirde beklenmeyen sonuçlar üretilebilir.
Multi-Thread okumayı desteklemek, bu koleksiyondan Row/Cell nesnelerine erişim performansını düşürebilir.
Lütfen bazı özelliklerin Multi-Thread okumayı destekleyemeyeceğini unutmayın.
biçimlendirme değerleri gibi ([Cell.string_value](/cells/tr/python-net/aspose.cells/cell#string_value), [Cell.display_string_value](/cells/tr/python-net/aspose.cells/cell#display_string_value), .vb. ile).
Dolayısıyla, bu özellik doğru olarak ayarlanmış olsa bile, bu API'ler yine de Multi-Thread okuma için beklenmeyen sonuçlar verebilir.
###  Tanım:
```python
@property
def multi_thread_reading(self):
    ...
@multi_thread_reading.setter
def multi_thread_reading(self, value):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Cells](/cells/tr/python-net/aspose.cells/cells)
