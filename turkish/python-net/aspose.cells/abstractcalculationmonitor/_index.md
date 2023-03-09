---
title: AbstractCalculationMonitor sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 30
url: /tr/python-net/aspose.cells/abstractcalculationmonitor/
is_root: false
---
##  AbstractCalculationMonitor sınıfı
Kullanıcının formül hesaplamasının ilerlemesini izlemesini izleyin.



AbstractCalculationMonitor türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [original_value](/cells/tr/python-net/aspose.cells/abstractcalculationmonitor/original_value) | Hesaplanan hücrenin eski değerini alır.<br/> Yalnızca [AbstractCalculationMonitor.before_calculate(sheet_index, row_index, col_index)](/cells/tr/python-net/aspose.cells/abstractcalculationmonitor/before_calculate) ve [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/tr/python-net/aspose.cells/abstractcalculationmonitor/after_calculate)'de kullanılmalıdır.|
| [value_changed](/cells/tr/python-net/aspose.cells/abstractcalculationmonitor/value_changed) | Hesaplamadan sonra hücrenin değerinin değişip değişmediği.<br/> Sadece [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/tr/python-net/aspose.cells/abstractcalculationmonitor/after_calculate)'de kullanılmalıdır.|
| [calculated_value](/cells/tr/python-net/aspose.cells/abstractcalculationmonitor/calculated_value) | Hücrenin yeni hesaplanan değerini alır.<br/> Sadece [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/tr/python-net/aspose.cells/abstractcalculationmonitor/after_calculate)'de kullanılmalıdır.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [before_calculate(sheet_index, row_index, col_index)](/cells/tr/python-net/aspose.cells/abstractcalculationmonitor/before_calculate/#int-int-int) | Bir hücreyi hesaplamadan önce iş yapmak için bu yöntemi uygulayın.|
| [after_calculate(sheet_index, row_index, col_index)](/cells/tr/python-net/aspose.cells/abstractcalculationmonitor/after_calculate/#int-int-int) | Bir hücre hesaplandıktan sonra iş yapmak için bu yöntemi uygulayın.|
| [on_circular(circular_cells_data)](/cells/tr/python-net/aspose.cells/abstractcalculationmonitor/on_circular/#collections.abc.Iterator) | Döngüsel referanslara sahip formülleri hesaplarken iş yapmak için bu yöntemi uygulayın.|



###  Ayrıca bakınız
* modül [aspose.cells](..)
