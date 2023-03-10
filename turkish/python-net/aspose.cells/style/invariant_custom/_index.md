---
title: invariant_custom mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 260
url: /tr/python-net/aspose.cells/style/invariant_custom/
is_root: false
---
##  invariant_custom mülk

Sayı biçimi için kültürden bağımsız desen dizesini alır.
Bu nesne için herhangi bir sayı biçimi ayarlanmamışsa, null döndürülür.
Sayı biçimi yerleşikse, yerleşik sayıya karşılık gelen kalıp dizisi döndürülür.

###  Notlar

Yerleşik sayı biçimleri için döndürülen kalıp içeriği hala kültüre bağlıdır,
örneğin, bazı yerel ayarlar için "m/d/y" ve diğer bazı yerel ayarlar için "d/m/y" döndürür.
[Style.culture_custom](/cells/tr/python-net/aspose.cells/style#culture_custom)'den farkı şudur (kültürden bağımsız olan da budur):
biçim belirticileri ve ayırıcılar standart olarak tutulur, '/' gibi her zaman tarih-saat ayırıcı olarak kullanılır
ve belirli yerel ayar için başka hangi özel karakter kullanılırsa kullanılsın, "y" her zaman "yıl" bölümü olarak kullanılacaktır.
###  Tanım:
```python
@property
def invariant_custom(self):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Style](/cells/tr/python-net/aspose.cells/style)
