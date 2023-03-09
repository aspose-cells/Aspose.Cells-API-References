---
title: start_row yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 60
url: /tr/python-net/aspose.cells/lightcellsdataprovider/start_row/
is_root: false
---
##  start_row(row) {#Row}
Bir satırın verilerini kaydetmeye başlar.



```python
def start_row(self, row):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| row | [Row](/cells/tr/python-net/aspose.cells/row) | Verileri doldurmak için uygulama için satır nesnesi. Satır dizini, [LightCellsDataProvider.next_row()](/cells/tr/python-net/aspose.cells/lightcellsdataprovider/next_row)'in son çağrısının döndürülen değeridir.<br/>Satır, iç hücreler modelinde başlatıldıysa, mevcut satır nesnesi kullanılacaktır.<br/> Aksi takdirde, verileri doldurmak için uygulama için geçici bir Row nesnesi kullanılacaktır.|
###  Notlar

Bir satırı ve hücre verilerini kaydetmenin başında çağrılacaktır.
Geçerli satırda yükseklik, stil vb. bazı özel özellikler varsa,
uygulama, bu özellikleri burada verilen Row nesnesine ayarlamalıdır.


###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [LightCellsDataProvider](/cells/tr/python-net/aspose.cells/lightcellsdataprovider)
