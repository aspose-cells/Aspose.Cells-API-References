---
title: FormatCondition sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 690
url: /tr/python-net/aspose.cells/formatcondition/
is_root: false
---
##  FormatCondition sınıf
Koşullu biçimlendirme koşulunu temsil eder.



FormatCondition türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [formula1](/cells/tr/python-net/aspose.cells/formatcondition/formula1) | Koşullu biçimlendirmeyle ilişkili değeri veya ifadeyi alır ve ayarlar.|
| [formula2](/cells/tr/python-net/aspose.cells/formatcondition/formula2) | Koşullu biçimlendirmeyle ilişkili değeri veya ifadeyi alır ve ayarlar.|
| [operator](/cells/tr/python-net/aspose.cells/formatcondition/operator) | Koşullu biçim işleç türünü alır ve ayarlar.|
| [stop_if_true](/cells/tr/python-net/aspose.cells/formatcondition/stop_if_true) | Doğru, bu kural doğru olarak değerlendirildiğinde, daha düşük önceliğe sahip hiçbir kural bu kurala uygulanamaz.<br/> Yalnızca Excel 2007 için geçerlidir;|
| [priority](/cells/tr/python-net/aspose.cells/formatcondition/priority) | Bu koşullu biçimlendirme kuralının önceliği. Bu değer hangisini belirlemek için kullanılır?<br/>biçimi değerlendirilmeli ve işlenmelidir. Daha düşük sayısal değerler daha yüksek önceliğe sahiptir.<br/> '1'in en yüksek öncelik olduğu daha yüksek sayısal değerler.|
| [style](/cells/tr/python-net/aspose.cells/formatcondition/style) | Koşullu biçimlendirilmiş hücre aralıklarının stilini alır veya ayarlar.|
| [type](/cells/tr/python-net/aspose.cells/formatcondition/type) | Alır ve koşullu biçim Type ayarlar.|
| [icon_set](/cells/tr/python-net/aspose.cells/formatcondition/icon_set) | Koşullu biçimlendirmenin "IconSet" örneğini alın.<br/>Varsayılan örneğin IconSetType'ı TrafficLights31'dir.<br/> Yalnızca type = IconSet için geçerlidir.|
| [data_bar](/cells/tr/python-net/aspose.cells/formatcondition/data_bar) | Koşullu biçimlendirmenin "DataBar" örneğini alın.<br/>Varsayılan örneğin rengi mavidir.<br/> Yalnızca tür için geçerli olan DataBar'dır.|
| [color_scale](/cells/tr/python-net/aspose.cells/formatcondition/color_scale) |Koşullu biçimlendirmenin "ColorScale" örneğini alın.<br/>Varsayılan örnek bir "yeşil-sarı-kırmızı" 3ColorScale'dir.<br/> Yalnızca type = ColorScale için geçerlidir.|
| [top10](/cells/tr/python-net/aspose.cells/formatcondition/top10) | Koşullu biçimlendirmenin "Top10" örneğini alın.<br/>Varsayılan örneğin kuralı,<br/>değerler ilk 10 parantez içinde yer alır.<br/> Sadece Top10 türü için geçerlidir.|
| [above_average](/cells/tr/python-net/aspose.cells/formatcondition/above_average) | Koşullu biçimlendirmenin "AboveAverage" örneğini alın.<br/> Varsayılan örneğin kuralı, şu hücreleri vurgular:<br/>aralıktaki tüm değerler için ortalamanın üzerinde.<br/> Yalnızca type = AboveAverage için geçerlidir.|
| [text](/cells/tr/python-net/aspose.cells/formatcondition/text) | Bir "metin içerir" koşullu biçimlendirme kuralındaki metin değeri.<br/>Yalnızca type = includeText, notContainsText, beginWith ve biterWith için geçerlidir.<br/> Varsayılan değer boştur.|
| [time_period](/cells/tr/python-net/aspose.cells/formatcondition/time_period) | Bir "tarih meydana geliyor..." koşullu biçimlendirme kuralında geçerli zaman aralığı.<br/>Yalnızca type = timePeriod için geçerlidir.<br/> Varsayılan değer TimePeriodType.Today'dir.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [get_formula1(is_r1c1, is_local)](/cells/tr/python-net/aspose.cells/formatcondition/get_formula1/#bool-bool) | Bu biçim koşuluyla ilişkili değeri veya ifadeyi alır.|
| [get_formula1(is_r1c1, is_local, row, column)](/cells/tr/python-net/aspose.cells/formatcondition/get_formula1/#bool-bool-int-int) |Hücrenin koşullu biçimlendirmesinin değerini veya ifadesini alır.|
| [get_formula1(row, column)](/cells/tr/python-net/aspose.cells/formatcondition/get_formula1/#int-int) | Hücrenin koşullu biçimlendirmesinin formülünü alır.|
| [get_formula2(is_r1c1, is_local)](/cells/tr/python-net/aspose.cells/formatcondition/get_formula2/#bool-bool) | Bu biçim koşuluyla ilişkili değeri veya ifadeyi alır.|
| [get_formula2(is_r1c1, is_local, row, column)](/cells/tr/python-net/aspose.cells/formatcondition/get_formula2/#bool-bool-int-int) |Hücrenin koşullu biçimlendirmesinin değerini veya ifadesini alır.|
| [get_formula2(row, column)](/cells/tr/python-net/aspose.cells/formatcondition/get_formula2/#int-int) | Hücrenin koşullu biçimlendirmesinin formülünü alır.|
| [set_formulas(formula1, formula2, is_r1c1, is_local)](/cells/tr/python-net/aspose.cells/formatcondition/set_formulas/#str-str-bool-bool) | Bu biçim koşuluyla ilişkili değeri veya ifadeyi ayarlar.|
| [set_formula1(formula, is_r1c1, is_local)](/cells/tr/python-net/aspose.cells/formatcondition/set_formula1/#str-bool-bool) | Bu biçim koşuluyla ilişkili değeri veya ifadeyi ayarlar.|
| [set_formula2(formula, is_r1c1, is_local)](/cells/tr/python-net/aspose.cells/formatcondition/set_formula2/#str-bool-bool) | Bu biçim koşuluyla ilişkili değeri veya ifadeyi ayarlar.|



###  Örnek

```python
from aspose.cells import CellArea, FormatConditionType, OperatorType, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea()
ca.start_row = 0
ca.end_row = 0
ca.start_column = 0
ca.end_column = 0
fcs.add_area(ca)
ca = CellArea()
ca.start_row = 1
ca.end_row = 1
ca.start_column = 1
ca.end_column = 1
fcs.add_area(ca)
# Adds condition.
conditionIndex = fcs.add_condition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100")
# Adds condition.
conditionIndex2 = fcs.add_condition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100")
# Sets the background color.
fc = fcs[conditionIndex]
fc.style.background_color = Color.red
# Saving the Excel file
workbook.save("output.xls")

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
