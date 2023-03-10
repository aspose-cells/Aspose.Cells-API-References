---
title: OdsLoadOptions класс
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 1100
url: /ru/python-net/aspose.cells/odsloadoptions/
is_root: false
---
##  OdsLoadOptions класс
Представляет параметры загрузки файла ods.



**Наследование:** [OdsLoadOptions](/cells/python-net/aspose.cells/odsloadoptions) → 
[LoadOptions](/cells/ru/python-net/aspose.cells/loadoptions)



Тип OdsLoadOptions предоставляет следующие члены:

###  Конструкторы
| Конструктор| Описание|
| :- | :- |
| [OdsLoadOptions()](/cells/ru/python-net/aspose.cells/odsloadoptions/__init__/#) | Представляет параметры загрузки файла ods.|
| [OdsLoadOptions(type)](/cells/ru/python-net/aspose.cells/odsloadoptions/__init__/#LoadFormat) | Представляет параметры загрузки файла ods.|


###  Характеристики
| Свойство| Описание|
| :- | :- |
| [load_format](/cells/ru/python-net/aspose.cells/odsloadoptions/load_format) | Получает формат загрузки.|
| [password](/cells/ru/python-net/aspose.cells/odsloadoptions/password) | Получает и устанавливает пароль книги.|
| [parsing_formula_on_open](/cells/ru/python-net/aspose.cells/odsloadoptions/parsing_formula_on_open) | Указывает, выполняется ли разбор формулы при чтении файла.|
| [parsing_pivot_cached_records](/cells/ru/python-net/aspose.cells/odsloadoptions/parsing_pivot_cached_records) | Указывает, выполняется ли разбор сводных кэшированных записей при загрузке файла.<br/> Значение по умолчанию неверно.|
| [language_code](/cells/ru/python-net/aspose.cells/odsloadoptions/language_code) | Получает или задает язык пользовательского интерфейса версии Workbook на основе CountryCode, в котором сохранен файл.|
| [region](/cells/ru/python-net/aspose.cells/odsloadoptions/region) | Получает или задает региональные параметры системы на основе CountryCode на момент загрузки файла.|
| [default_style_settings](/cells/ru/python-net/aspose.cells/odsloadoptions/default_style_settings) | Получает параметры стиля по умолчанию для инициализации стилей книги.|
| [standard_font](/cells/ru/python-net/aspose.cells/odsloadoptions/standard_font) | Устанавливает стандартное имя шрифта по умолчанию|
| [standard_font_size](/cells/ru/python-net/aspose.cells/odsloadoptions/standard_font_size) | Устанавливает стандартный размер шрифта по умолчанию.|
| [interrupt_monitor](/cells/ru/python-net/aspose.cells/odsloadoptions/interrupt_monitor) | Получает и устанавливает монитор прерываний.|
| [ignore_not_printed](/cells/ru/python-net/aspose.cells/odsloadoptions/ignore_not_printed) | Игнорировать данные, которые не печатаются, при прямой печати файла|
| [check_data_valid](/cells/ru/python-net/aspose.cells/odsloadoptions/check_data_valid) |Проверьте правильность данных в файле шаблона.|
| [check_excel_restriction](/cells/ru/python-net/aspose.cells/odsloadoptions/check_excel_restriction) | Проверять ли ограничение файла excel, когда пользователь изменяет объекты, связанные с ячейками.<br/>Например, Excel не позволяет вводить строковое значение длиннее 32 КБ.<br/>Когда вы вводите значение длиннее 32 КБ, например, Cell.PutValue(строка), если это свойство истинно, вы получите исключение.<br/>Если это свойство имеет значение false, мы примем значение вашей входной строки в качестве значения ячейки, чтобы позже<br/>вы можете вывести полное строковое значение для файлов других форматов, таких как CSV.<br/>Однако, если вы установили такое значение, которое недопустимо для формата файла Excel,<br/> вы не должны сохранять книгу в формате файла Excel позже. В противном случае может возникнуть непредвиденная ошибка для сгенерированного файла Excel.|
| [keep_unparsed_data](/cells/ru/python-net/aspose.cells/odsloadoptions/keep_unparsed_data) | Сохранять ли непроанализированные данные в памяти для рабочей книги, когда она загружается из файла шаблона. Значение по умолчанию верно.|
| [load_filter](/cells/ru/python-net/aspose.cells/odsloadoptions/load_filter) | Фильтр для обозначения того, как загружать данные.|
| [light_cells_data_handler](/cells/ru/python-net/aspose.cells/odsloadoptions/light_cells_data_handler) | Обработчик данных для обработки данных ячеек при чтении файла шаблона.|
| [memory_setting](/cells/ru/python-net/aspose.cells/odsloadoptions/memory_setting) | Получает или задает параметры использования памяти.|
| [warning_callback](/cells/ru/python-net/aspose.cells/odsloadoptions/warning_callback) | Получает или задает обратный вызов предупреждения.|
| [auto_fitter_options](/cells/ru/python-net/aspose.cells/odsloadoptions/auto_fitter_options) | Получает и задает параметры автоматической установки|
| [auto_filter](/cells/ru/python-net/aspose.cells/odsloadoptions/auto_filter) | Указывает, выполняется ли автоматическая фильтрация данных при загрузке файлов.|
| [font_configs](/cells/ru/python-net/aspose.cells/odsloadoptions/font_configs) | Получает и устанавливает отдельные конфигурации шрифтов.<br/> Работает только для [Workbook](/cells/ru/python-net/aspose.cells/workbook), который использует этот [LoadOptions](/cells/ru/python-net/aspose.cells/loadoptions) для загрузки.|
| [apply_excel_default_style_to_hyperlink](/cells/ru/python-net/aspose.cells/odsloadoptions/apply_excel_default_style_to_hyperlink) | Указывает, применяется ли стиль Excel по умолчанию к гиперссылке.|
| [refresh_pivot_tables](/cells/ru/python-net/aspose.cells/odsloadoptions/refresh_pivot_tables) | Указывает, обновляются ли сводные таблицы при загрузке файла.|


###  Методы
| Метод| Описание|
| :- | :- |
| [set_paper_size(type)](/cells/ru/python-net/aspose.cells/odsloadoptions/set_paper_size/#PaperSizeType) | Устанавливает размер бумаги для печати по умолчанию из настроек принтера по умолчанию.|



###  Смотрите также
* модуль [aspose.cells](..)
* класс [LoadOptions](/cells/ru/python-net/aspose.cells/loadoptions)
* класс [OdsLoadOptions](/cells/ru/python-net/aspose.cells/odsloadoptions)
* класс [Workbook](/cells/ru/python-net/aspose.cells/workbook)
