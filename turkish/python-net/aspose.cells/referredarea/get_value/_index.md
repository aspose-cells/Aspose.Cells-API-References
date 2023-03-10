---
title: get_value yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells/referredarea/get_value/
is_root: false
---
##  get_value(row_offset, col_offset) {#int-int}
Bu alanın sol üst köşesinden verilen ofset ile hücre değerini alır.


###  İadeler

"#REF!" bu alan geçersiz ise;
Bu alanın dışında ofset verilirse "#N/A";
Aksi takdirde, hücre değerini verilen konumda döndürün.


```python
def get_value(self, row_offset, col_offset):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| row_offset | int | bu alanın başlangıç satırından satır ofseti|
| col_offset | int |bu alanın başlangıç satırından sütun uzaklığı|


##  get_value(row_offset, col_offset, calculate_formulas) {#int-int-bool}
Bu alanın sol üst köşesinden verilen ofset ile hücre değerini alır.


###  İadeler

"#REF!" bu alan geçersiz ise;
Bu alanın dışında ofset verilirse "#N/A";
Aksi takdirde, hücre değerini verilen konumda döndürün.


```python
def get_value(self, row_offset, col_offset, calculate_formulas):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| row_offset | int | bu alanın başlangıç satırından satır ofseti|
| col_offset | int |bu alanın başlangıç satırından sütun uzaklığı|
| calculate_formulas | bool | Belirtilen başvuru formül ise yinelemeli olarak hesaplanıp hesaplanmadığı|



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [ReferredArea](/cells/tr/python-net/aspose.cells/referredarea)
