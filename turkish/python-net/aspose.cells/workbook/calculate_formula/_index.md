---
title: calculate_formula yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 40
url: /tr/python-net/aspose.cells/workbook/calculate_formula/
is_root: false
---
##  calculate_formula() {#}
Formüllerin sonucunu hesaplar.



```python
def calculate_formula(self):
    ...
```


###  Notlar

Desteklenen tüm formüller için lütfen https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions adresindeki listeye bakın.

##  calculate_formula(ignore_error) {#bool}

Formüllerin sonucunu hesaplar.



```python
def calculate_formula(self, ignore_error):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| ignore_error | bool | Formüllerin hesaplanmasındaki hatayı gizleyip gizlemediğini gösterir. Hata, desteklenmeyen işlev, harici bağlantılar vb. olabilir.|


##  calculate_formula(options) {#CalculationOptions}
Bu çalışma kitabında formüllerin hesaplanması.



```python
def calculate_formula(self, options):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| options | [CalculationOptions](/cells/tr/python-net/aspose.cells/calculationoptions) | Hesaplama seçenekleri|


##  calculate_formula(ignore_error, custom_function) {#bool-ICustomFunction}
Formüllerin sonucunu hesaplar.



```python
def calculate_formula(self, ignore_error, custom_function):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| ignore_error | bool | Formüllerin hesaplanmasındaki hatayı gizleyip gizlemediğini gösterir. Hata, desteklenmeyen işlev, harici bağlantılar vb. olabilir.|
| custom_function | [ICustomFunction](/cells/tr/python-net/aspose.cells/icustomfunction) | Özel formül hesaplama, hesaplama motorunu genişletmek için çalışır.|
###  Notlar

NOT: Bu üye artık kullanılmıyor. Yerine,
lütfen CalculateFormula(CalculationOptions) yöntemini kullanın.
 Bu yöntem Ağustos 2020'den itibaren 12 ay sonra kaldırılacaktır.
Aspose yaşamış olabileceğiniz rahatsızlıktan dolayı özür diler.


###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [Workbook](/cells/tr/python-net/aspose.cells/workbook)
