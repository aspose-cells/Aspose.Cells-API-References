---
title: calculation_mode mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 60
url: /tr/python-net/aspose.cells/formulasettings/calculation_mode/
is_root: false
---
##  calculation_mode mülk

Ms excel'de çalışma kitabı hesaplama modunu alır veya ayarlar.

###  Notlar

Bu özellik, yalnızca ayarları sonuçtaki elektronik tablo dosyasına kaydetmek içindir
böylece diğer uygulamalar (ms excel gibi) ortaya çıkan dosyayı yüklerken ve değiştirirken buna göre hareket edebilir.
Çoğu kullanıcının uygulamasında performans değerlendirmesi için, çalışma kitabındaki hiçbir formülü otomatik olarak hesaplamayız,
bu özellik için hangi modun ayarlandığı önemli değildir.
Kullanıcının formülleri hesaplaması gerekiyorsa, lütfen her zaman gereksinime göre farklı nesnelerdeki yöntemleri çağırın:
[Workbook.calculate_formula()](/cells/python-net/aspose.cells/workbook/calculate_formula), [Worksheet.calculate_formula(formula)](/cells/python-net/aspose.cells/worksheet/calculate_formula),
[Cell.calculate(options)](/cells/tr/python-net/aspose.cells/cell/calculate), ...vb.
###  Tanım:
```python
@property
def calculation_mode(self):
    ...
@calculation_mode.setter
def calculation_mode(self, value):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells](../../)
* sınıf [CalcModeType](/cells/tr/python-net/aspose.cells/calcmodetype)
* sınıf [FormulaSettings](/cells/tr/python-net/aspose.cells/formulasettings)
