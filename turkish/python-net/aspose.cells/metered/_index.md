---
title: Metered sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 1050
url: /tr/python-net/aspose.cells/metered/
is_root: false
---
##  Metered sınıf
Ölçülen anahtarı ayarlamak için yöntemler sağlar.



Metered türü aşağıdaki üyeleri gösterir:

###  İnşaatçılar
| Yapıcı| Tanım|
| :- | :- |
| [Metered()](/cells/tr/python-net/aspose.cells/metered/__init__/#) | Bu sınıfın yeni bir örneğini başlatır.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [set_metered_key(public_key, private_key)](/cells/tr/python-net/aspose.cells/metered/set_metered_key/#str-str) | Tarifeli genel ve özel anahtarı ayarlar.<br/> Sayaçlı lisans satın alıyorsanız, uygulamayı başlattığınızda bu API aranmalıdır, normalde bu yeterlidir. Ancak, tüketim verilerini her zaman yükleyemezseniz ve 24 saati aşarsanız, lisans değerlendirme durumuna alınır, böyle bir durumla karşılaşmamak için lisans durumunu düzenli olarak kontrol etmelisiniz, değerlendirme durumuysa, bu API'i tekrar arayın.|
| [get_consumption_quantity()](/cells/tr/python-net/aspose.cells/metered/get_consumption_quantity/#) | Tüketim dosyası boyutunu alır|
| [get_consumption_credit()](/cells/tr/python-net/aspose.cells/metered/get_consumption_credit/#) | Tüketim kredisi alıyor|



###  Örnek

Bu örnekte ölçülü genel ve özel anahtar ayarlanmaya çalışılacaktır.


```python
from aspose.cells import Metered

matered = Metered()
matered.set_metered_key("PublicKey", "PrivateKey")

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
