---
title: start_sheet yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 70
url: /tr/python-net/aspose.cells/lightcellsdataprovider/start_sheet/
is_root: false
---
##  start_sheet(sheet_index) {#int}
Bir çalışma sayfasını kaydetmeye başlar.


###  İadeler

true bu sağlayıcı verilen sayfa için veri sağlayacaksa; false eğer verilen sayfa normal veri modelini kullanmalıdır(Cells).


```python
def start_sheet(self, sheet_index):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| sheet_index | int | kaydedilecek geçerli sayfanın dizini.|
###  Notlar

Bir çalışma kitabının kaydedilmesi sırasında bir çalışma sayfasının kaydedilmesinin başında çağrılacaktır.
 Sağlayıcının başvurması gerekiyorsa*"sayfa dizini"* Daha sonra
startRow(Row) veya startCell(Cell) yönteminde,
 yani, sürecin hangi çalışma sayfasının işlenmekte olduğunu bilmesi gerekiyorsa,
 uygulama şu özellikleri korumalıdır:*"sayfa dizini"* burada değer.


###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [LightCellsDataProvider](/cells/tr/python-net/aspose.cells/lightcellsdataprovider)
