---
title: FormatCondition klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 690
url: /sv/python-net/aspose.cells/formatcondition/
is_root: false
---
##  FormatCondition klass
Representerar villkorligt formateringsvillkor.



Typen FormatCondition avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [formula1](/cells/sv/python-net/aspose.cells/formatcondition/formula1) | Hämtar och ställer in värdet eller uttrycket som är kopplat till villkorlig formatering.|
| [formula2](/cells/sv/python-net/aspose.cells/formatcondition/formula2) | Hämtar och ställer in värdet eller uttrycket som är kopplat till villkorlig formatering.|
| [operator](/cells/sv/python-net/aspose.cells/formatcondition/operator) | Hämtar och ställer in operatortypen för villkorsformat.|
| [stop_if_true](/cells/sv/python-net/aspose.cells/formatcondition/stop_if_true) |Det är sant att inga regler med lägre prioritet kan tillämpas över denna regel när denna regel utvärderas till sann.<br/> Gäller endast Excel 2007;|
| [priority](/cells/sv/python-net/aspose.cells/formatcondition/priority) | Prioriteten för denna villkorliga formateringsregel. Detta värde används för att bestämma vilken<br/>formatet bör utvärderas och återges. Lägre numeriska värden har högre prioritet än<br/> högre numeriska värden, där '1' har högsta prioritet.|
| [style](/cells/sv/python-net/aspose.cells/formatcondition/style) | Hämtar eller ställer in stil för villkorligt formaterade cellområden.|
| [type](/cells/sv/python-net/aspose.cells/formatcondition/type) | Hämtar och ställer in om det villkorliga formatet Typ.|
| [icon_set](/cells/sv/python-net/aspose.cells/formatcondition/icon_set) | Hämta den villkorliga formateringens "IconSet"-instans.<br/>Standardinstansens IconSetType är TrafficLights31.<br/> Gäller endast för typ = IconSet.|
| [data_bar](/cells/sv/python-net/aspose.cells/formatcondition/data_bar) | Hämta den villkorliga formateringens "DataBar"-instans.<br/>Standardinstansens färg är blå.<br/> Endast giltig för typ är DataBar.|
| [color_scale](/cells/sv/python-net/aspose.cells/formatcondition/color_scale) | Hämta den villkorliga formateringens "ColorScale"-instans.<br/>Standardinstansen är en "grön-gul-röd" 3ColorScale .<br/> Gäller endast för typ = ColorScale.|
| [top10](/cells/sv/python-net/aspose.cells/formatcondition/top10) | Hämta den villkorliga formateringens "Top10"-instans.<br/>Standardinstansens regel markerar celler vars<br/>värden hamnar i topp 10-parentesen.<br/> Gäller endast för typ är Top10.|
| [above_average](/cells/sv/python-net/aspose.cells/formatcondition/above_average) |Hämta den villkorliga formateringens "AboveAverage"-instans.<br/> Standardinstansens regel markerar celler som är<br/>över genomsnittet för alla värden i intervallet.<br/> Gäller endast för typ = Övermedel.|
| [text](/cells/sv/python-net/aspose.cells/formatcondition/text) | Textvärdet i en regel för villkorlig formatering "text innehåller".<br/>Gäller endast för typen = innehåller text, inte innehåller text, börjar med och slutar med.<br/> Standardvärdet är null.|
| [time_period](/cells/sv/python-net/aspose.cells/formatcondition/time_period) | Den tillämpliga tidsperioden i en "datum inträffar..." villkorlig formateringsregel.<br/>Gäller endast för typ = timePeriod.<br/> Standardvärdet är TimePeriodType.Today.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [get_formula1(is_r1c1, is_local)](/cells/sv/python-net/aspose.cells/formatcondition/get_formula1/#bool-bool) | Hämtar värdet eller uttrycket som är kopplat till detta formatvillkor.|
| [get_formula1(is_r1c1, is_local, row, column)](/cells/sv/python-net/aspose.cells/formatcondition/get_formula1/#bool-bool-int-int) | Hämtar värdet eller uttrycket för den villkorliga formateringen av cellen.|
| [get_formula1(row, column)](/cells/sv/python-net/aspose.cells/formatcondition/get_formula1/#int-int) | Hämtar formeln för den villkorliga formateringen av cellen.|
| [get_formula2(is_r1c1, is_local)](/cells/sv/python-net/aspose.cells/formatcondition/get_formula2/#bool-bool) | Hämtar värdet eller uttrycket som är kopplat till detta formatvillkor.|
| [get_formula2(is_r1c1, is_local, row, column)](/cells/sv/python-net/aspose.cells/formatcondition/get_formula2/#bool-bool-int-int) | Hämtar värdet eller uttrycket för den villkorliga formateringen av cellen.|
| [get_formula2(row, column)](/cells/sv/python-net/aspose.cells/formatcondition/get_formula2/#int-int) | Hämtar formeln för den villkorliga formateringen av cellen.|
| [set_formulas(formula1, formula2, is_r1c1, is_local)](/cells/sv/python-net/aspose.cells/formatcondition/set_formulas/#str-str-bool-bool) | Ställer in värdet eller uttrycket som är associerat med detta formatvillkor.|
| [set_formula1(formula, is_r1c1, is_local)](/cells/sv/python-net/aspose.cells/formatcondition/set_formula1/#str-bool-bool) | Ställer in värdet eller uttrycket som är associerat med detta formatvillkor.|
| [set_formula2(formula, is_r1c1, is_local)](/cells/sv/python-net/aspose.cells/formatcondition/set_formula2/#str-bool-bool) | Ställer in värdet eller uttrycket som är associerat med detta formatvillkor.|



###  Exempel

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

###  Se även
* modul [aspose.cells](..)
