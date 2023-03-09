---
title: Metered sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 1050
url: /tr/python-net/aspose.cells/metered/
is_root: false
---
##  Metered sınıfı
Ölçülen anahtarları ayarlamak için yöntemler sağlar.



Metered türü aşağıdaki üyeleri gösterir:

###  İnşaatçılar
| Yapıcı| Tanım|
| :- | :- |
| [Metered()](/cells/tr/python-net/aspose.cells/metered/__init__/#) | Bu sınıfın yeni bir örneğini başlatır.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [set_metered_key(public_key, private_key)](/cells/tr/python-net/aspose.cells/metered/set_metered_key/#str-str) | Tarifeli genel ve özel anahtarları ayarlar.<br/>Tarifeli lisans alıyorsanız başvuruyu başlatırken bu API aranmalı normalde bu yeterlidir lisans durumunu düzenli olarak kontrol etmelisiniz değerlendirme durumu ise tekrar API arayınız.|
| [get_consumption_quantity()](/cells/tr/python-net/aspose.cells/metered/get_consumption_quantity/#) | Tüketim dosyası boyutunu alır|
| [get_consumption_credit()](/cells/tr/python-net/aspose.cells/metered/get_consumption_credit/#) | Tüketim kredisi alıyor|



###  örnekler

Bu örnekte ölçülü genel ve özel anahtarlar ayarlanmaya çalışılacaktır.


```python
from aspose.cells import Metered

matered = Metered()
matered.set_metered_key("PublicKey", "PrivateKey")

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
