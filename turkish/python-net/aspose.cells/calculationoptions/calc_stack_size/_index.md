---
title: calc_stack_size mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 30
url: /tr/python-net/aspose.cells/calculationoptions/calc_stack_size/
is_root: false
---
##  calc_stack_size mülk

Hücreleri yinelemeli olarak hesaplamak için yığın boyutunu belirtir.

###  Notlar

Bağımlılık ağacında yinelemeli olarak hesaplanması gereken çok sayıda hücre olduğunda,
StackOverflowException, hesaplama sürecinde ortaya çıkabilir.
Eğer öyleyse, kullanıcı bu özellik için daha küçük bir değer belirtmelidir.
Bu tür durumlar için kullanıcı, gerçek formüllere ve verilere göre bu özellik için uygun değeri belirlemelidir.
Çok küçük değerler, formül hesaplaması için performansın düşmesine neden olabilir.
###  Tanım:
```python
@property
def calc_stack_size(self):
    ...
@calc_stack_size.setter
def calc_stack_size(self, value):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [CalculationOptions](/cells/tr/python-net/aspose.cells/calculationoptions)
