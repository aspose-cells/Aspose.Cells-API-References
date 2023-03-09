---
title: change_palette yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 50
url: /tr/python-net/aspose.cells/workbook/change_palette/
is_root: false
---
##  change_palette(color, index) {#aspose.pydrawing.Color-int}
Belirtilen dizindeki elektronik tablonun paletini değiştirir.



```python
def change_palette(self, color, index):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| color | aspose.pydrawing.Color | Renk yapısı.|
| index | int | Palet dizini, 0 - 55.|
###  Notlar

Palette, her biri bir RGB değeriyle temsil edilen 56 giriş vardır.


Palette olmayan bir renk ayarlarsanız etkili olmaz.


Bu nedenle, özel bir renk ayarlamak istiyorsanız, lütfen önce paleti değiştirin.


Aşağıdaki standart renk paletidir.

| Renk| Kırmızı| Yeşil| Mavi|
| :- | :- | :- | :- |
| Siyah| 0| 0| 0 |
| Beyaz| 255| 255| 255 |
| Kırmızı| 255| 0| 0 |
| Kireç| 0| 255| 0 |
| Mavi| 0| 0| 255 |
| Sarı| 255| 255| 0 |
| eflatun| 255| 0| 255 |
| camgöbeği| 0| 255| 255 |
| bordo| 128| 0| 0 |
| Yeşil| 0| 128| 0 |
| Donanma| 0| 0| 128 |
| zeytin| 128| 128| 0 |
| Mor| 128| 0| 128 |
| deniz mavisi| 0| 128| 128 |
| Gümüş| 192| 192| 192 |
| Gri| 128| 128| 128 |
| Renk17| 153| 153| 255 |
| Renk18| 153| 51| 102 |
| Renk19| 255| 255| 204 |
| Renk20| 204| 255| 255 |
| Renk21| 102| 0| 102 |
| Renk22| 255| 128| 128 |
| Renk23| 0| 102| 204 |
| Renk24| 204| 204| 255 |
| Renk25| 0| 0| 128 |
| Renk26| 255| 0| 255 |
| Renk27| 255| 255| 0 |
| Renk28| 0| 255| 255 |
| Renk29| 128| 0| 128 |
| Renk30| 128| 0| 0 |
| Renk31| 0| 128| 128 |
| Renk32| 0| 0| 255 |
| Renk33| 0| 204| 255 |
| Renk34| 204| 255| 255 |
| Renk35| 204| 255| 204 |
| Renk36| 255| 255| 153 |
| Renk37| 153| 204| 255 |
| Renk38| 255| 153| 204 |
| Renk39| 204| 153| 255 |
| Renk40| 255| 204| 153 |
| Renk41| 51| 102| 255 |
| Renk42| 51| 204| 204 |
| Renk43| 153| 204| 0 |
| Renk44| 255| 204| 0 |
| Renk45| 255| 153| 0 |
| Renk46| 255| 102| 0 |
| Renk47| 102| 102| 153 |
| Renk48| 150| 150| 150 |
| Renk49| 0| 51| 102 |
| Renk50| 51| 153| 102 |
| Renk51| 0| 51| 0 |
| Renk52| 51| 51| 0 |
| Renk53| 153| 51| 0 |
|Renk54| 153| 51| 102 |
| Renk55| 51| 51| 153 |
| Renk56| 51| 51| 51 |


###  Ayrıca bakınız

* modül [aspose.cells](../../)
* sınıf [Workbook](/cells/tr/python-net/aspose.cells/workbook)
