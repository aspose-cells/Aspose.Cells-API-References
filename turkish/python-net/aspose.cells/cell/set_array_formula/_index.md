---
title: set_array_formula yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 290
url: /tr/python-net/aspose.cells/cell/set_array_formula/
is_root: false
---
##  set_array_formula(array_formula, row_number, column_number) {#str-int-int}
Bir dizi formülünü (ms excel'de CTRL+SHIFT+ENTER ile girilen eski dizi formülü) bir hücre aralığına ayarlar.



```python
def set_array_formula(self, array_formula, row_number, column_number):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| array_formula | str | Dizi formülü.|
| row_number | int | Dizi formülünün sonucunun doldurulacağı satır sayısı.|
| column_number | int | Dizi formülünün sonucunu dolduracak sütun sayısı.|


##  set_array_formula(array_formula, row_number, column_number, options) {#str-int-int-FormulaParseOptions}
Bir dizi formülünü bir hücre aralığına ayarlar.



```python
def set_array_formula(self, array_formula, row_number, column_number, options):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| array_formula | str | Dizi formülü.|
| row_number | int | Dizi formülünün sonucunun doldurulacağı satır sayısı.|
| column_number | int | Dizi formülünün sonucunu dolduracak sütun sayısı.|
| options | [FormulaParseOptions](/cells/tr/python-net/aspose.cells/formulaparseoptions) | Formülü ayrıştırma seçenekleri.|


##  set_array_formula(array_formula, row_number, column_number, is_r1c1, is_local) {#str-int-int-bool-bool}
Bir dizi formülünü bir hücre aralığına ayarlar.



```python
def set_array_formula(self, array_formula, row_number, column_number, is_r1c1, is_local):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| array_formula | str | Dizi formülü.|
| row_number | int | Dizi formülünün sonucunun doldurulacağı satır sayısı.|
| column_number | int | Dizi formülünün sonucunu dolduracak sütun sayısı.|
| is_r1c1 | bool | formülün R1C1 formülü olup olmadığı|
| is_local | bool | formülün yerel biçimlendirilmiş olup olmadığı|
###  Notlar

NOT: Bu sınıf artık kullanılmıyor. Yerine,
lütfen Cell.SetArrayFormula(string,int,int,FormulaParseOptions) kullanın.
Bu mülk, Aralık 2019'dan bu yana 12 ay sonra kaldırılacaktır.
Aspose yaşamış olabileceğiniz rahatsızlıktan dolayı özür diler.

##  set_array_formula(array_formula, row_number, column_number, options, values) {#str-int-int-FormulaParseOptions-list}
Bir dizi formülünü bir hücre aralığına ayarlar.



```python
def set_array_formula(self, array_formula, row_number, column_number, options, values):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| array_formula | str | Dizi formülü.|
| row_number | int | Dizi formülünün sonucunun doldurulacağı satır sayısı.|
| column_number | int | Dizi formülünün sonucunu dolduracak sütun sayısı.|
| options | [FormulaParseOptions](/cells/tr/python-net/aspose.cells/formulaparseoptions) | Formülü ayrıştırma seçenekleri.|
| values | list | verilen dizi formülü ile bu hücreler için değerler|



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Cell](/cells/tr/python-net/aspose.cells/cell)
