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
Böyle bir durumda, kullanıcı bu özellik için uygun değeri gerçek formüllere ve verilere göre belirlemelidir.
Çok küçük bir değer, formül hesaplamasında performansın düşmesine neden olabilir.
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
