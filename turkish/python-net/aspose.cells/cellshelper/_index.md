---
title: CellsHelper sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 230
url: /tr/python-net/aspose.cells/cellshelper/
is_root: false
---
##  CellsHelper sınıfı
Yardımcı işlevler sağlar.



CellsHelper türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [significant_digits](/cells/tr/python-net/aspose.cells/cellshelper/significant_digits) | Anlamlı basamak sayısını alır ve ayarlar.<br/> Varsayılan değer 17'dir.|
| [dpi](/cells/tr/python-net/aspose.cells/cellshelper/dpi) | Makinenin DPI'sini alır.|
| [startup_path](/cells/tr/python-net/aspose.cells/cellshelper/startup_path) |Bazı dış formül başvuruları tarafından başvurulan başlangıç yolunu alır veya ayarlar.|
| [alt_start_path](/cells/tr/python-net/aspose.cells/cellshelper/alt_start_path) | Bazı harici formül başvuruları tarafından başvurulan alternatif başlangıç yolunu alır veya ayarlar.|
| [library_path](/cells/tr/python-net/aspose.cells/cellshelper/library_path) | Bazı dış formül başvuruları tarafından başvurulan kitaplık yolunu alır veya ayarlar.|
| [custom_implementation_factory](/cells/tr/python-net/aspose.cells/cellshelper/custom_implementation_factory) | Özel uygulama ile örnekler oluşturmak için fabrikayı alır veya ayarlar.|
| [is_cloud_platform](/cells/tr/python-net/aspose.cells/cellshelper/is_cloud_platform) | Azure, AWSLambda vb. gibi bir bulut platformunda çalışırken lütfen bu özelliği True olarak ayarlayın.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [create_safe_sheet_name(name_proposal)](/cells/tr/python-net/aspose.cells/cellshelper/create_safe_sheet_name/#str) | Verilen sayfa adını kontrol eder ve gerektiğinde geçerli bir tane oluşturur.<br/>Verilen sayfa adı excel sayfa adı kurallarına uygunsa iade edin.<br/>Aksi takdirde, uzunluk sınırı aşarsa dize kesilir<br/> ve geçersiz karakterler '' ile değiştirilecek, ardından yeniden oluşturulmuş dize değerini döndürecektir.|
| [create_safe_sheet_name(name_proposal, replace_char)](/cells/tr/python-net/aspose.cells/cellshelper/create_safe_sheet_name/#str-char) | Verilen sayfa adını kontrol eder ve gerektiğinde geçerli bir tane oluşturur.<br/>Verilen sayfa adı excel sayfa adı kurallarına uygunsa iade edin.<br/>Aksi takdirde, uzunluk sınırı aşarsa dize kesilir<br/> ve geçersiz karakterler verilen karakterle değiştirilecek, ardından yeniden oluşturulmuş dize değerini döndürecektir.|
| [get_text_width(text, font, scaling)](/cells/tr/python-net/aspose.cells/cellshelper/get_text_width/#str-Font-float) | Nokta birimi cinsinden metnin genişliğini alın.|
| [get_version()](/cells/tr/python-net/aspose.cells/cellshelper/get_version/#) | Yayın sürümünü edinin.|
| [cell_name_to_index(cell_name, row, column)](/cells/tr/python-net/aspose.cells/cellshelper/cell_name_to_index/#str-any-any) | Adına göre hücre satır ve sütun dizinlerini alır.|
| [cell_index_to_name(row, column)](/cells/tr/python-net/aspose.cells/cellshelper/cell_index_to_name/#int-int) | Satır ve sütun indekslerine göre hücre adını alır.|
| [column_index_to_name(column)](/cells/tr/python-net/aspose.cells/cellshelper/column_index_to_name/#int) | Sütun indeksine göre sütun adını alır.|
| [column_name_to_index(column_name)](/cells/tr/python-net/aspose.cells/cellshelper/column_name_to_index/#str) |Sütun adına göre sütun dizini alır.|
| [row_index_to_name(row)](/cells/tr/python-net/aspose.cells/cellshelper/row_index_to_name/#int) | Satır dizinine göre satır adını alır.|
| [row_name_to_index(row_name)](/cells/tr/python-net/aspose.cells/cellshelper/row_name_to_index/#str) | Satır adına göre satır indeksi alır.|
| [convert_r1c1_formula_to_a1(r_1c1_formula, row, column)](/cells/tr/python-net/aspose.cells/cellshelper/convert_r1c1_formula_to_a1/#str-int-int) | Hücrenin r1c1 formülünü A1 formülüne dönüştürür.|
| [convert_a1_formula_to_r1c1(formula, row, column)](/cells/tr/python-net/aspose.cells/cellshelper/convert_a1_formula_to_r1c1/#str-int-int) | Hücrenin A1 formülünü r1c1 formülüne dönüştürür.|
| [get_date_time_from_double(double_value, date1904)](/cells/tr/python-net/aspose.cells/cellshelper/get_date_time_from_double/#float-bool) | Double değerini tarih saat değerine dönüştürün.|
| [get_double_from_date_time(date_time, date1904)](/cells/tr/python-net/aspose.cells/cellshelper/get_double_from_date_time/#DateTime-bool) | Tarih saatini çift değere dönüştürün.|
| [get_used_colors(workbook)](/cells/tr/python-net/aspose.cells/cellshelper/get_used_colors/#Workbook) | Çalışma kitabında kullanılan tüm renkleri alır.|
| [add_add_in_function(function, min_count_of_parameters, max_count_of_parameters, paramers_type, function_value_type)](/cells/tr/python-net/aspose.cells/cellshelper/add_add_in_function/#str-int-int-list-ParameterType) | Eklenti işlevi ekleyin.|
| [merge_files(files, cached_file, dest_file)](/cells/tr/python-net/aspose.cells/cellshelper/merge_files/#list-str-str) | Bazı büyük xls dosyalarını bir xls dosyasında birleştirir.|
| [init_for_dot_net_core()](/cells/tr/python-net/aspose.cells/cellshelper/init_for_dot_net_core/#) | .NetCore programı için başlatma işlemini yapın.<br/> Tüm .NetCore başlatma işlemleri için önce bu yöntemi çağırmanızı öneririz.<br/>Örneğin:<br/>CellsHelper.InitForDotNetCore();<br/> Çalışma kitabı wb = yeni Çalışma Kitabı();|



###  Ayrıca bakınız
* modül [aspose.cells](..)
