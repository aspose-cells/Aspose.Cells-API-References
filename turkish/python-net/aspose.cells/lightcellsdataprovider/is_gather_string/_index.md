---
title: is_gather_string yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells/lightcellsdataprovider/is_gather_string/
is_root: false
---
##  is_gather_string() {#}
Hücrenin geçerli dize değerinin genel bir havuzda toplanması gerekip gerekmediğini kontrol eder.


###  İadeler

true sonuç dosyası için bir genel havuzda dize değerinin toplanması gerekiyorsa.


```python
def is_gather_string(self):
    ...
```


###  Notlar

Dize değerlerinin toplanması, yalnızca bu uygulama tarafından sağlanan hücreler için çok sayıda yinelenen dize değeri olduğunda avantaj sağlar.
Bu durumda dize toplamak, çok fazla bellek tasarrufu sağlayacak ve daha küçük sonuç dosyası oluşturacaktır.
LightCellsDataProvider tarafından sağlanan hücreler için çok sayıda dize değeri varsa ancak bunlardan birkaçı aynıysa,
dize toplamak daha fazla belleğe ve zamana mal olur ve sonuçta ortaya çıkan dosya için hiçbir avantajı yoktur.


###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [LightCellsDataProvider](/cells/tr/python-net/aspose.cells/lightcellsdataprovider)
