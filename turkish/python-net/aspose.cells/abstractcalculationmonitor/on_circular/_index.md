---
title: on_circular yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 40
url: /tr/python-net/aspose.cells/abstractcalculationmonitor/on_circular/
is_root: false
---
##  on_circular(circular_cells_data) {#collections.abc.Iterator}
Döngüsel referanslara sahip formülleri hesaplarken iş yapmak için bu yöntemi uygulayın.


###  İadeler

Formül motorunun bu aramadan sonra bu hücreleri döngüsel olarak hesaplaması gerekip gerekmediği.
True, formül motorunun onlar için hesaplama yapmaya devam etmesine izin verir.
Formül motorunun bu hücreleri Hesaplanmış olarak işaretlemesine izin vermek için yanlış.


```python
def on_circular(self, circular_cells_data):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| circular_cells_data | collections.abc.Iterator | CalculationCell ile IEnumerator hücreleri temsil eden öğeler<br/> döngüsel referanslara bağlıdır.|
###  Notlar

Uygulamada kullanıcı, beklenen değeri hesaplanan sonuç olarak da ayarlayabilir.
bu hücrelerin bir kısmı/tümü için, böylece formül motoru bunları yinelemeli olarak hesaplamaz.


###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [AbstractCalculationMonitor](/cells/tr/python-net/aspose.cells/abstractcalculationmonitor)
