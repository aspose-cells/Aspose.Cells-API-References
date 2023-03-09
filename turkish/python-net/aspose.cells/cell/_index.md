---
title: Cell sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 140
url: /tr/python-net/aspose.cells/cell/
is_root: false
---
##  Cell sınıfı
Tek bir Çalışma Kitabı hücresini temsil eden nesneyi kapsüller.



Cell türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [worksheet](/cells/tr/python-net/aspose.cells/cell/worksheet) | Üst çalışma sayfasını alır.|
| [date_time_value](/cells/tr/python-net/aspose.cells/cell/date_time_value) | Hücrede bulunan DateTime değerini alır.|
| [row](/cells/tr/python-net/aspose.cells/cell/row) | Hücrenin satır numarasını (sıfır tabanlı) alır.|
| [column](/cells/tr/python-net/aspose.cells/cell/column) | Hücrenin sütun numarasını (sıfır tabanlı) alır.|
| [is_formula](/cells/tr/python-net/aspose.cells/cell/is_formula) | Belirtilen hücrenin formül içerip içermediğini temsil eder.|
| [type](/cells/tr/python-net/aspose.cells/cell/type) | Hücre değeri türünü temsil eder.|
| [name](/cells/tr/python-net/aspose.cells/cell/name) | Hücrenin adını alır.|
| [is_error_value](/cells/tr/python-net/aspose.cells/cell/is_error_value) | Bu hücrenin değerinin bir hata olup olmadığını kontrol eder.|
| [is_numeric_value](/cells/tr/python-net/aspose.cells/cell/is_numeric_value) | Bu hücrenin iç değerinin sayısal (int, double ve datetime) olup olmadığını gösterir.|
| [string_value](/cells/tr/python-net/aspose.cells/cell/string_value) |Hücrede bulunan dize değerini alır.<br/>Diğer hücre türleri için biçimlendirilmiş dize değeri (bu hücrenin belirtilen stiliyle biçimlendirilmiş) döndürülür.<br/>Biçimlendirilmiş hücre değeri, bir hücreyi metin olarak kopyalarken excel'den alabileceğiniz değerle aynıdır (örneğin,<br/> hücreyi metin düzenleyiciye kopyalama veya csv'ye aktarma).|
| [string_value_without_format](/cells/tr/python-net/aspose.cells/cell/string_value_without_format) | Herhangi bir format olmadan hücrenin değerini string olarak alır.|
| [number_category_type](/cells/tr/python-net/aspose.cells/cell/number_category_type) | Bu hücrenin sayı biçimlendirmesinin kategori türünü temsil eder.|
| [display_string_value](/cells/tr/python-net/aspose.cells/cell/display_string_value) | Hücrenin görüntü stiline göre bu hücrenin biçimlendirilmiş dize değerini alır.|
| [int_value](/cells/tr/python-net/aspose.cells/cell/int_value) | Hücrede bulunan tamsayı değerini alır.|
| [double_value](/cells/tr/python-net/aspose.cells/cell/double_value) | Hücrede bulunan çift değeri alır.|
| [float_value](/cells/tr/python-net/aspose.cells/cell/float_value) | Hücrede bulunan kayan değeri alır.|
| [bool_value](/cells/tr/python-net/aspose.cells/cell/bool_value) | Hücrede bulunan boole değerini alır.|
| [has_custom_style](/cells/tr/python-net/aspose.cells/cell/has_custom_style) | Bu hücrenin özel stil ayarlarına sahip olup olmadığını gösterir (varsayılandan farklı, devralınan<br/> karşılık gelen satır, sütun veya çalışma kitabından).|
| [shared_style_index](/cells/tr/python-net/aspose.cells/cell/shared_style_index) | Stil havuzunda hücrenin paylaşılan stil dizinini alır.|
| [formula](/cells/tr/python-net/aspose.cells/cell/formula) | [Cell](/cells/tr/python-net/aspose.cells/cell) formülünü alır veya ayarlar.|
| [formula_local](/cells/tr/python-net/aspose.cells/cell/formula_local) | Hücrenin yerel olarak biçimlendirilmiş formülünü alın.|
| [r1c1_formula](/cells/tr/python-net/aspose.cells/cell/r1c1_formula) | [Cell](/cells/tr/python-net/aspose.cells/cell)'in bir R1C1 formülünü alır veya ayarlar.|
| [contains_external_link](/cells/tr/python-net/aspose.cells/cell/contains_external_link) |Bu hücrenin harici bir bağlantı içerip içermediğini gösterir.<br/> Yalnızca hücre bir formül hücresi olduğunda geçerlidir.|
| [is_array_header](/cells/tr/python-net/aspose.cells/cell/is_array_header) | Hücrenin formülünü ve dizi formülünü gösterir<br/> ve dizinin ilk hücresidir.|
| [is_dynamic_array_formula](/cells/tr/python-net/aspose.cells/cell/is_dynamic_array_formula) | Hücre formülünün dinamik dizi formülü(true) veya eski dizi formülü(false) olduğunu gösterir.|
| [is_array_formula](/cells/tr/python-net/aspose.cells/cell/is_array_formula) | Hücre formülünün bir dizi formülü olup olmadığını gösterir.|
| [is_in_array](/cells/tr/python-net/aspose.cells/cell/is_in_array) | Hücre formülünün bir dizi formülü olup olmadığını gösterir.|
| [is_shared_formula](/cells/tr/python-net/aspose.cells/cell/is_shared_formula) | Hücre formülünün paylaşılan bir formülün parçası olup olmadığını gösterir.|
| [is_table_formula](/cells/tr/python-net/aspose.cells/cell/is_table_formula) | Bu hücrenin tablo formülünün parçası olup olmadığını gösterir.|
| [is_in_table](/cells/tr/python-net/aspose.cells/cell/is_in_table) | Bu hücrenin tablo formülünün parçası olup olmadığını gösterir.|
| [value](/cells/tr/python-net/aspose.cells/cell/value) | Bu hücrede bulunan değeri alır.|
| [is_style_set](/cells/tr/python-net/aspose.cells/cell/is_style_set) | Hücrenin stilinin ayarlanıp ayarlanmadığını gösterir. false döndürürse, bu hücrenin varsayılan bir hücre formatına sahip olduğu anlamına gelir.|
| [is_merged](/cells/tr/python-net/aspose.cells/cell/is_merged) | Bir hücrenin birleştirilmiş bir aralığın parçası olup olmadığını kontrol eder.|
| [comment](/cells/tr/python-net/aspose.cells/cell/comment) | Bu hücrenin yorumunu alır.|
| [html_string](/cells/tr/python-net/aspose.cells/cell/html_string) | Bu hücrede veri ve bazı formatları içeren html dizisini alır ve ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [calculate(options)](/cells/tr/python-net/aspose.cells/cell/calculate/#CalculationOptions) | Hücrenin formülünü hesaplar.|
| [calculate(ignore_error, custom_function)](/cells/tr/python-net/aspose.cells/cell/calculate/#bool-ICustomFunction) | Hücrenin formülünü hesaplar.|
| [put_value(bool_value)](/cells/tr/python-net/aspose.cells/cell/put_value/#bool) | Hücreye bir boole değeri koyar.|
| [put_value(int_value)](/cells/tr/python-net/aspose.cells/cell/put_value/#int) | Hücreye bir tamsayı değeri koyar.|
| [put_value(double_value)](/cells/tr/python-net/aspose.cells/cell/put_value/#float) |Hücreye çift değer koyar.|
| [put_value(string_value, is_converted, set_style)](/cells/tr/python-net/aspose.cells/cell/put_value/#str-bool-bool) | Hücreye bir değer koyar, uygunsa bu değer diğer veri tipine çevrilir ve hücrenin sayı formatı sıfırlanır.|
| [put_value(string_value, is_converted)](/cells/tr/python-net/aspose.cells/cell/put_value/#str-bool) | Hücreye bir dize değeri koyar ve uygunsa değeri diğer veri türüne dönüştürür.|
| [put_value(string_value)](/cells/tr/python-net/aspose.cells/cell/put_value/#str) | Hücreye bir dize değeri koyar.|
| [put_value(date_time)](/cells/tr/python-net/aspose.cells/cell/put_value/#DateTime) | Hücreye bir DateTime değeri koyar.|
| [put_value(object_value)](/cells/tr/python-net/aspose.cells/cell/put_value/#any) | Hücreye bir nesne değeri koyar.|
| [get_display_style()](/cells/tr/python-net/aspose.cells/cell/get_display_style/#) | Hücrenin görüntü stilini alır.<br/>Bu hücre, koşullu biçimlendirme, liste nesneleri vb. gibi diğer ayarlardan da etkileniyorsa,<br/> o zaman görüntüleme stili cell.GetStyle()'dan farklı olabilir.|
| [get_display_style(include_merged_borders)](/cells/tr/python-net/aspose.cells/cell/get_display_style/#bool) | Hücrenin görüntü stilini alır.<br/> Hücre koşullu olarak biçimlendirilmişse, görüntüleme stili cell.GetStyle() ile aynı değildir.|
| [get_style()](/cells/tr/python-net/aspose.cells/cell/get_style/#) | Hücre stilini alır.|
| [get_style(check_borders)](/cells/tr/python-net/aspose.cells/cell/get_style/#bool) | CheckBorders doğruysa, diğer hücrelerin kenarlıklarının bu hücrenin stilini etkileyip etkilemediğini kontrol edin.|
| [set_style(style)](/cells/tr/python-net/aspose.cells/cell/set_style/#Style) | Hücre stilini ayarlar.|
| [set_style(style, explicit_flag)](/cells/tr/python-net/aspose.cells/cell/set_style/#Style-bool) | Hücre stilini uygulayın.|
| [set_style(style, flag)](/cells/tr/python-net/aspose.cells/cell/set_style/#Style-StyleFlag) | Hücre stilini uygulayın.|
| [set_formula(formula, value)](/cells/tr/python-net/aspose.cells/cell/set_formula/#str-any) | Formülü ve formülün değerini ayarlayın.|
| [set_formula(formula, is_r1c1, is_local, value)](/cells/tr/python-net/aspose.cells/cell/set_formula/#str-bool-bool-any) | Formülü ve formülün değerini ayarlayın.|
| [set_formula(formula, options, value)](/cells/tr/python-net/aspose.cells/cell/set_formula/#str-FormulaParseOptions-any) | Formülü ve formülün değerini ayarlayın.|
| [set_array_formula(array_formula, row_number, column_number, is_r1c1, is_local)](/cells/tr/python-net/aspose.cells/cell/set_array_formula/#str-int-int-bool-bool) | Bir dizi formülünü bir hücre aralığına ayarlar.|
| [set_array_formula(array_formula, row_number, column_number)](/cells/tr/python-net/aspose.cells/cell/set_array_formula/#str-int-int) |Bir dizi formülünü (ms excel'de CTRL+SHIFT+ENTER ile girilen eski dizi formülü) bir hücre aralığına ayarlar.|
| [set_array_formula(array_formula, row_number, column_number, options)](/cells/tr/python-net/aspose.cells/cell/set_array_formula/#str-int-int-FormulaParseOptions) | Bir dizi formülünü bir hücre aralığına ayarlar.|
| [set_array_formula(array_formula, row_number, column_number, options, values)](/cells/tr/python-net/aspose.cells/cell/set_array_formula/#str-int-int-FormulaParseOptions-list) | Bir dizi formülünü bir hücre aralığına ayarlar.|
| [set_shared_formula(shared_formula, row_number, column_number, is_r1c1, is_local)](/cells/tr/python-net/aspose.cells/cell/set_shared_formula/#str-int-int-bool-bool) | Formülü bir hücre aralığına ayarlar.|
| [set_shared_formula(shared_formula, row_number, column_number)](/cells/tr/python-net/aspose.cells/cell/set_shared_formula/#str-int-int) | Paylaşılan formülleri bir hücre aralığına ayarlar.|
| [set_shared_formula(shared_formula, row_number, column_number, options)](/cells/tr/python-net/aspose.cells/cell/set_shared_formula/#str-int-int-FormulaParseOptions) | Paylaşılan formülleri bir hücre aralığına ayarlar.|
| [set_shared_formula(shared_formula, row_number, column_number, options, values)](/cells/tr/python-net/aspose.cells/cell/set_shared_formula/#str-int-int-FormulaParseOptions-list) | Paylaşılan formülleri bir hücre aralığına ayarlar.|
| [get_leafs()](/cells/tr/python-net/aspose.cells/cell/get_leafs/#) | Doğrudan bu hücreye başvuran ve bu hücre değiştirildiğinde güncellenmesi gereken tüm hücreleri alın.|
| [get_leafs(recursive)](/cells/tr/python-net/aspose.cells/cell/get_leafs/#bool) | Bu hücre değiştirildiğinde güncellenecek olan tüm hücreleri alın.|
| [set_dynamic_array_formula(array_formula, options, calculate_value)](/cells/tr/python-net/aspose.cells/cell/set_dynamic_array_formula/#str-FormulaParseOptions-bool) | Dinamik dizi formülünü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar.|
| [set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value)](/cells/tr/python-net/aspose.cells/cell/set_dynamic_array_formula/#str-FormulaParseOptions-list-bool-bool) | Dinamik dizi formülünü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar.|
| [set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value, copts)](/cells/tr/python-net/aspose.cells/cell/set_dynamic_array_formula/#str-FormulaParseOptions-list-bool-bool-CalculationOptions) | Dinamik dizi formülünü ayarlar ve mümkünse formülün komşu hücrelere yayılmasını sağlar.|
| [set_table_formula(row_number, column_number, row_input_cell, column_input_cell, values)](/cells/tr/python-net/aspose.cells/cell/set_table_formula/#int-int-str-str-list) | Bu hücreden başlayarak belirli bir aralık için iki değişkenli bir veri tablosu oluşturun.|
| [set_table_formula(row_number, column_number, input_cell, is_row_input, values)](/cells/tr/python-net/aspose.cells/cell/set_table_formula/#int-int-str-bool-list) | Bu hücreden başlayarak verilen aralık için tek değişkenli veri tablosu oluşturun.|
| [set_table_formula(row_number, column_number, row_index_of_row_input_cell, column_index_of_row_input_cell, row_index_of_column_input_cell, column_index_of_column_input_cell, values)](/cells/tr/python-net/aspose.cells/cell/set_table_formula/#int-int-int-int-int-int-list) | Bu hücreden başlayarak belirli bir aralık için iki değişkenli bir veri tablosu oluşturun.|
| [set_table_formula(row_number, column_number, row_index_of_input_cell, column_index_of_input_cell, is_row_input, values)](/cells/tr/python-net/aspose.cells/cell/set_table_formula/#int-int-int-int-bool-list) | Bu hücreden başlayarak verilen aralık için tek değişkenli veri tablosu oluşturun.|
| [get_characters()](/cells/tr/python-net/aspose.cells/cell/get_characters/#) | Tüm Karakterler nesnelerini döndürür<br/> hücre metni içindeki bir karakter aralığını temsil eder.|
| [get_characters(flag)](/cells/tr/python-net/aspose.cells/cell/get_characters/#bool) | Tüm Karakterler nesnelerini döndürür<br/> hücre metni içindeki bir karakter aralığını temsil eder.|
| [get_string_value(format_strategy)](/cells/tr/python-net/aspose.cells/cell/get_string_value/#CellValueFormatStrategy) | Dize değerini belirli biçimlendirilmiş stratejiye göre alır.|
| [get_width_of_value()](/cells/tr/python-net/aspose.cells/cell/get_width_of_value/#) | Değerin genişliğini piksel cinsinden alır.|
| [get_height_of_value()](/cells/tr/python-net/aspose.cells/cell/get_height_of_value/#) | Değerin yüksekliğini piksel cinsinden alır.|
| [get_format_conditions()](/cells/tr/python-net/aspose.cells/cell/get_format_conditions/#) | Bu hücreye uygulanan biçim koşullarını alır.|
| [get_formula(is_r1c1, is_local)](/cells/tr/python-net/aspose.cells/cell/get_formula/#bool-bool) | Bu hücrenin formülünü alın.|
| [get_precedents()](/cells/tr/python-net/aspose.cells/cell/get_precedents/#) |Bu hücrenin formülünde görünen tüm başvuruları alır.|
| [get_dependents(is_all)](/cells/tr/python-net/aspose.cells/cell/get_dependents/#bool) | Formülü doğrudan bu hücreye başvuran tüm hücreleri alın.|
| [get_precedents_in_calculation()](/cells/tr/python-net/aspose.cells/cell/get_precedents_in_calculation/#) | Hesaplarken bu hücrenin formülü tarafından kullanılan tüm emsalleri (mevcut çalışma kitabındaki hücrelere referans) alır.|
| [get_dependents_in_calculation(recursive)](/cells/tr/python-net/aspose.cells/cell/get_dependents_in_calculation/#bool) | Hesaplanan sonucu bu hücreye bağlı olan tüm hücreleri alır.|
| [get_array_range()](/cells/tr/python-net/aspose.cells/cell/get_array_range/#) | Hücrenin formülü bir dizi formülü ise dizi aralığını alır.|
| [remove_array_formula(leave_normal_formula)](/cells/tr/python-net/aspose.cells/cell/remove_array_formula/#bool) | Dizi formülünü kaldırın.|
| [copy(cell)](/cells/tr/python-net/aspose.cells/cell/copy/#Cell) | Verileri bir kaynak hücreden kopyalar.|
| [characters(start_index, length)](/cells/tr/python-net/aspose.cells/cell/characters/#int-int) | Hücre metni içindeki bir karakter aralığını temsil eden bir Characters nesnesi döndürür.|
| [is_rich_text()](/cells/tr/python-net/aspose.cells/cell/is_rich_text/#) | Hücre dizesi değerinin zengin bir metin olup olmadığını gösterir.|
| [set_characters(characters)](/cells/tr/python-net/aspose.cells/cell/set_characters/#list) | Hücrenin zengin metin biçimini ayarlar.|
| [get_merged_range()](/cells/tr/python-net/aspose.cells/cell/get_merged_range/#) | Birleştirilmiş bir aralığı temsil eden [Range](/cells/tr/python-net/aspose.cells/range) nesnesini döndürür.|
| [get_html_string(html5)](/cells/tr/python-net/aspose.cells/cell/get_html_string/#bool) | Bu hücrede veri ve bazı formatları içeren html dizisini alır.|
| [to_json()](/cells/tr/python-net/aspose.cells/cell/to_json/#) | [Cell](/cells/tr/python-net/aspose.cells/cell)'i JSON yapı verisine dönüştürün.|
| [equals(cell)](/cells/tr/python-net/aspose.cells/cell/equals/#Cell) | Bu nesnenin, başka bir hücre nesnesiyle aynı hücreye atıfta bulunup bulunmadığını kontrol eder.|
| [get_conditional_formatting_result()](/cells/tr/python-net/aspose.cells/cell/get_conditional_formatting_result/#) | Koşullu biçimlendirmenin sonucunu alın.|
| [get_validation()](/cells/tr/python-net/aspose.cells/cell/get_validation/#) |Bu hücreye uygulanan doğrulamayı alır.|
| [get_validation_value()](/cells/tr/python-net/aspose.cells/cell/get_validation_value/#) | Bu hücreye uygulanan doğrulama değerini alır.|
| [get_table()](/cells/tr/python-net/aspose.cells/cell/get_table/#) | Bu hücreyi içeren tabloyu alır.|



###  örnekler

```python
from aspose.cells import TextAlignmentType, Workbook
from aspose.pydrawing import Color

excel = Workbook()
cells = excel.worksheets[0].cells
# Put a string into a cell
cell = cells.get(0, 0)
cell.put_value("Hello")
first = cell.string_value
# Put an integer into a cell
cell = cells.get("B1")
cell.put_value(12)
second = cell.int_value
# Put a double into a cell
cell = cells.get(0, 2)
cell.put_value(-1.234)
third = cell.double_value
# Put a formula into a cell
cell = cells.get("D1")
cell.formula = "=B1 + C1"
# Put a combined formula: "sum(average(b1,c1), b1)" to cell at b2
cell = cells.get("b2")
cell.formula = "=sum(average(b1,c1), b1)"
# Set style of a cell
style = cell.get_style()
# Set background color
style.background_color = Color.yellow
# Set format of a cell
style.font.name = "Courier New"
style.vertical_alignment = TextAlignmentType.TOP
cell.set_style(style)

```

###  Ayrıca bakınız
* modül [aspose.cells](..)
* sınıf [Cell](/cells/tr/python-net/aspose.cells/cell)
* sınıf [Range](/cells/tr/python-net/aspose.cells/range)
