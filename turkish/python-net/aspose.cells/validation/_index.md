---
title: Validation sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 1540
url: /tr/python-net/aspose.cells/validation/
is_root: false
---
##  Validation sınıfı
Veri validation.settings'i temsil eder.



Validation türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [operator](/cells/tr/python-net/aspose.cells/validation/operator) | Veri doğrulama için işleci temsil eder.|
| [alert_style](/cells/tr/python-net/aspose.cells/validation/alert_style) | Doğrulama uyarı stilini temsil eder.|
| [type](/cells/tr/python-net/aspose.cells/validation/type) | Veri doğrulama türünü temsil eder.|
| [input_message](/cells/tr/python-net/aspose.cells/validation/input_message) | Veri doğrulama giriş mesajını temsil eder.|
| [input_title](/cells/tr/python-net/aspose.cells/validation/input_title) | Veri doğrulama giriş iletişim kutusunun başlığını temsil eder.|
| [error_message](/cells/tr/python-net/aspose.cells/validation/error_message) | Veri doğrulama hata mesajını temsil eder.|
| [error_title](/cells/tr/python-net/aspose.cells/validation/error_title) | Veri doğrulama hatası iletişim kutusunun başlığını temsil eder.|
| [show_input](/cells/tr/python-net/aspose.cells/validation/show_input) |Kullanıcı veri doğrulama aralığında bir hücre seçtiğinde veri doğrulama giriş mesajının görüntülenip görüntülenmeyeceğini belirtir.|
| [show_error](/cells/tr/python-net/aspose.cells/validation/show_error) | Kullanıcı geçersiz veri girdiğinde veri doğrulama hata mesajının görüntülenip görüntülenmeyeceğini belirtir.|
| [ignore_blank](/cells/tr/python-net/aspose.cells/validation/ignore_blank) | Aralık veri doğrulaması tarafından boş değerlere izin verilip verilmediğini gösterir.|
| [formula1](/cells/tr/python-net/aspose.cells/validation/formula1) | Veri doğrulamayla ilişkili değeri veya ifadeyi temsil eder.|
| [formula2](/cells/tr/python-net/aspose.cells/validation/formula2) | Veri doğrulamayla ilişkili değeri veya ifadeyi temsil eder.|
| [value1](/cells/tr/python-net/aspose.cells/validation/value1) | Veri doğrulamayla ilişkili ilk değeri temsil eder.|
| [value2](/cells/tr/python-net/aspose.cells/validation/value2) | Veri doğrulamayla ilişkili ikinci değeri temsil eder.|
| [in_cell_drop_down](/cells/tr/python-net/aspose.cells/validation/in_cell_drop_down) | Veri doğrulamanın kabul edilebilir değerler içeren bir açılır liste gösterip göstermediğini belirtir.|
| [areas](/cells/tr/python-net/aspose.cells/validation/areas) | Veri doğrulama ayarlarını içeren tüm [CellArea](/cells/tr/python-net/aspose.cells/cellarea)'i alır.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [get_formula1(is_r1c1, is_local)](/cells/tr/python-net/aspose.cells/validation/get_formula1/#bool-bool) | Bu doğrulamayla ilişkili değeri veya ifadeyi alır.|
| [get_formula1(is_r1c1, is_local, row, column)](/cells/tr/python-net/aspose.cells/validation/get_formula1/#bool-bool-int-int) | Belirli hücre için bu doğrulamayla ilişkili değeri veya ifadeyi alır.|
| [get_formula2(is_r1c1, is_local)](/cells/tr/python-net/aspose.cells/validation/get_formula2/#bool-bool) | Bu doğrulamayla ilişkili değeri veya ifadeyi alır.|
| [get_formula2(is_r1c1, is_local, row, column)](/cells/tr/python-net/aspose.cells/validation/get_formula2/#bool-bool-int-int) | Belirli hücre için bu doğrulamayla ilişkili değeri veya ifadeyi alır.|
| [add_area(cell_area)](/cells/tr/python-net/aspose.cells/validation/add_area/#CellArea) | Doğrulamayı alana uygular.|
| [add_area(cell_area, check_intersection, check_edge)](/cells/tr/python-net/aspose.cells/validation/add_area/#CellArea-bool-bool) | Doğrulamayı alana uygular.|
| [set_formula1(formula, is_r1c1, is_local)](/cells/tr/python-net/aspose.cells/validation/set_formula1/#str-bool-bool) | Bu doğrulama ile ilişkili değeri veya ifadeyi ayarlar.|
| [set_formula2(formula, is_r1c1, is_local)](/cells/tr/python-net/aspose.cells/validation/set_formula2/#str-bool-bool) | Bu doğrulama ile ilişkili değeri veya ifadeyi ayarlar.|
| [get_list_value(row, column)](/cells/tr/python-net/aspose.cells/validation/get_list_value/#int-int) |Belirtilen hücre için doğrulama listesi için değeri alın.|
| [add_areas(areas, check_intersection, check_edge)](/cells/tr/python-net/aspose.cells/validation/add_areas/#list-bool-bool) | Doğrulamayı verilen alanlara uygular.|
| [remove_area(cell_area)](/cells/tr/python-net/aspose.cells/validation/remove_area/#CellArea) | Aralıktaki doğrulama ayarlarını kaldırın.|
| [remove_areas(areas)](/cells/tr/python-net/aspose.cells/validation/remove_areas/#list) | Bu doğrulamayı verilen alanlardan kaldırır.|
| [remove_a_cell(row, column)](/cells/tr/python-net/aspose.cells/validation/remove_a_cell/#int-int) | Hücredeki doğrulama ayarlarını kaldırın.|
| [copy(source, copy_option)](/cells/tr/python-net/aspose.cells/validation/copy/#Validation-CopyOptions) | Doğrulamayı kopyala.|



###  örnekler

```python
from aspose.cells import CellArea, OperatorType, ValidationType, Workbook

workbook = Workbook()
validations = workbook.worksheets[0].validations
area = CellArea.create_cell_area(0, 0, 1, 1)
validation = validations[validations.add(area)]
validation.type = ValidationType.WHOLE_NUMBER
validation.operator = OperatorType.BETWEEN
validation.formula1 = "3"
validation.formula2 = "1234"

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
* sınıf [CellArea](/cells/tr/python-net/aspose.cells/cellarea)
