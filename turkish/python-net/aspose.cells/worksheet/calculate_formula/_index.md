---
title: calculate_formula yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 80
url: /tr/python-net/aspose.cells/worksheet/calculate_formula/
is_root: false
---
##  calculate_formula(formula) {#str}
Bir formül hesaplar.


###  İadeler

Hesaplanan formül sonucu.


```python
def calculate_formula(self, formula):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| formula | str | Hesaplanacak formül.|


##  calculate_formula(formula, opts) {#str-CalculationOptions}
Bir formül hesaplar.


###  İadeler

Hesaplanan formül sonucu.


```python
def calculate_formula(self, formula, opts):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| formula | str | Hesaplanacak formül.|
| opts | [CalculationOptions](/cells/tr/python-net/aspose.cells/calculationoptions) | Formül hesaplama seçenekleri|


##  calculate_formula(options, recursive) {#CalculationOptions-bool}
Bu çalışma sayfasındaki tüm formülleri hesaplar.



```python
def calculate_formula(self, options, recursive):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| options | [CalculationOptions](/cells/tr/python-net/aspose.cells/calculationoptions) | Hesaplama seçenekleri|
| recursive | bool | Doğru, çalışma sayfasının hücrelerinin diğer çalışma sayfalarının hücrelerine bağımlı olması anlamına gelir,<br/>diğer çalışma sayfalarındaki bağımlı hücreler de hesaplanacaktır.<br/> Yanlış, çalışma sayfasındaki tüm formüllerin hesaplandığı ve değerlerin doğru olduğu anlamına gelir.|


##  calculate_formula(recursive, ignore_error, custom_function) {#bool-bool-ICustomFunction}
Bu çalışma sayfasındaki tüm formülleri hesaplar.



```python
def calculate_formula(self, recursive, ignore_error, custom_function):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| recursive | bool | Doğru, çalışma sayfasının hücrelerinin diğer çalışma sayfalarının hücrelerine bağımlı olması anlamına gelir,<br/>diğer çalışma sayfalarındaki bağımlı hücreler de hesaplanacaktır.<br/> Yanlış, çalışma sayfasındaki tüm formüllerin hesaplandığı ve değerlerin doğru olduğu anlamına gelir.|
| ignore_error | bool | Formüllerin hesaplanmasındaki hatayı gizleyip gizlemediğini gösterir.<br/> Hata, desteklenmeyen işlevler, harici bağlantılar vb. olabilir.|
| custom_function | [ICustomFunction](/cells/tr/python-net/aspose.cells/icustomfunction) | Özel formül hesaplama, hesaplama motorunu genişletmek için çalışır.|
###  Notlar

NOT: Bu üye artık kullanılmıyor.
lütfen CalculateFormula(CalculationOptions, bool) yöntemini kullanın.
 Bu yöntem Ağustos 2020'den itibaren 12 ay sonra kaldırılacaktır.
Aspose yaşamış olabileceğiniz rahatsızlıktan dolayı özür diler.


###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Worksheet](/cells/tr/python-net/aspose.cells/worksheet)
