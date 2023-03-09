---
title: set_dynamic_array_formula yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 310
url: /tr/python-net/aspose.cells/cell/set_dynamic_array_formula/
is_root: false
---
##  set_dynamic_array_formula(array_formula, options, calculate_value) {#str-FormulaParseOptions-bool}
Dinamik dizi formülünü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar.


###  İadeler

formülün içine girmesi gereken aralık.


```python
def set_dynamic_array_formula(self, array_formula, options, calculate_value):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| array_formula | str | formül ifadesi|
| options | [FormulaParseOptions](/cells/tr/python-net/aspose.cells/formulaparseoptions) | formülü ayrıştırmak için seçenekler.<br/> "Ayrıştır" seçeneği göz ardı edilecek ve formül her zaman hemen ayrıştırılacaktır.|
| calculate_value | bool | taşan aralıktaki bu hücreler için bu dinamik dizi formülünün hesaplanıp hesaplanmayacağını.|


##  set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value) {#str-FormulaParseOptions-list-bool-bool}
Dinamik dizi formülünü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar.


###  İadeler

formülün içine girmesi gereken aralık.


```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| array_formula | str | formül ifadesi|
| options | [FormulaParseOptions](/cells/tr/python-net/aspose.cells/formulaparseoptions) | formülü ayrıştırmak için seçenekler.<br/> "Ayrıştır" seçeneği göz ardı edilecek ve formül her zaman hemen ayrıştırılacaktır.|
| values | list |verilen dinamik dizi formülü ile bu hücreler için değerler|
| calculate_range | bool | Bu dinamik dizi formülü için taşan aralığın hesaplanıp hesaplanmayacağı.<br/>"values" parametresi null değilse ve bu bayrak yanlışsa,<br/> sonra taşan aralığın yüksekliği değerler olur. Uzunluk ve genişlik değerler [0]. Uzunluk olur.|
| calculate_value | bool | "değerler" boş olduğunda, taşan aralıktaki hücreler için bu dinamik dizi formülünün hesaplanıp hesaplanmadığı<br/> veya bir hücre için "değerler"deki karşılık gelen öğe boştur.|


##  set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value, copts) {#str-FormulaParseOptions-list-bool-bool-CalculationOptions}
Dinamik dizi formülünü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar.


###  İadeler

formülün içine girmesi gereken aralık.


```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value, copts):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| array_formula | str | formül ifadesi|
| options | [FormulaParseOptions](/cells/tr/python-net/aspose.cells/formulaparseoptions) | formülü ayrıştırmak için seçenekler.<br/> "Ayrıştır" seçeneği göz ardı edilecek ve formül her zaman hemen ayrıştırılacaktır.|
| values | list |verilen dinamik dizi formülü ile bu hücreler için değerler|
| calculate_range | bool | Bu dinamik dizi formülü için taşan aralığın hesaplanıp hesaplanmayacağı.<br/>"values" parametresi null değilse ve bu bayrak yanlışsa,<br/> sonra taşan aralığın yüksekliği değerler olur. Uzunluk ve genişlik değerler [0]. Uzunluk olur.|
| calculate_value | bool | "değerler" boş olduğunda, taşan aralıktaki hücreler için bu dinamik dizi formülünün hesaplanıp hesaplanmadığı<br/> veya bir hücre için "değerler"deki karşılık gelen öğe boştur.|
| copts | [CalculationOptions](/cells/tr/python-net/aspose.cells/calculationoptions) | Formül hesaplama seçenekleri.<br/> Genel olarak, performans değerlendirmesi için [CalculationOptions.recursive](/cells/tr/python-net/aspose.cells/calculationoptions#recursive) özelliği false olmalıdır.|



###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Cell](/cells/tr/python-net/aspose.cells/cell)
