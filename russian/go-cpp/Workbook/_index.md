---
title: "Класс Workbook"
linktitle: "Workbook"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс Workbook. Инкапсулирует объект, представляющий workbook в Go."
type: docs
weight: 200
url: /ru/go-cpp/workbook/
---

## Workbook class

Представляет корневой объект для создания электронной таблицы Excel.

```go

type Workbook struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewWorkbook](./newworkbook/) | Инициализирует новый экземпляр класса Workbook. |
| [NewWorkbook_FileFormatType](./newworkbook_fileformattype/) | Инициализирует новый экземпляр класса Workbook. |
| [NewWorkbook_LoadOptions](./newworkbook_loadoptions/) | Инициализирует новый пустой экземпляр класса Workbook с параметрами. |
| [NewWorkbook_String](./newworkbook_string/) | Инициализирует новый экземпляр класса Workbook и открывает файл. |
| [NewWorkbook_Stream](./newworkbook_stream/) | Инициализирует новый экземпляр класса Workbook и открывает поток. |
| [NewWorkbook_String_LoadOptions](./newworkbook_string_loadoptions/) | Инициализирует новый экземпляр класса Workbook и открывает файл. |
| [NewWorkbook_Stream_LoadOptions](./newworkbook_stream_loadoptions/) | Инициализирует новый экземпляр класса Workbook и открывает поток. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetSettings](./getsettings/) | Представляет настройки рабочей книги. |
| [ParseFormulas](./parseformulas/) | Разбирает все формулы, которые не были разобраны при загрузке из шаблонного файла или при установке в ячейку. |
| [StartAccessCache](./startaccesscache/) | Запускает сеанс, использующий кэши для доступа к данным. |
| [CloseAccessCache](./closeaccesscache/) | Закрывает сеанс, использующий кэши для доступа к данным. |
| [Save_String_SaveFormat](./save_string_saveformat/) | Сохраняет книгу на диск. |
| [Save_String](./save_string/) | Сохранить книгу на диск. |
| [Save_String_SaveOptions](./save_string_saveoptions/) | Сохраняет книгу на диск. |
| [Save_SaveFormat](./save_saveformat/) | Сохраняет книгу в поток. |
| [Save_SaveOptions](./save_saveoptions/) | Сохраняет книгу в поток. |
| [SaveToStream](./savetostream/) | Сохраняет файл Excel в объект MemoryStream как файл Excel97-2003 xls и возвращает его. |
| [GetWorksheets](./getworksheets/) | Получает коллекцию WorksheetCollection в электронной таблице. |
| [IsLicensed](./islicensed/) | Указывает, установлена ли лицензия. |
| [RemoveUnusedStyles](./removeunusedstyles/) | Удалить все неиспользуемые стили. |
| [CreateStyle](./createstyle/) | Создаёт новый стиль. |
| [CreateStyle_Bool](./createstyle_bool/) | Создаёт новый стиль. |
| [CreateBuiltinStyle](./createbuiltinstyle/) | Создаёт встроенный стиль по заданному типу. |
| [CreateCellsColor](./createcellscolor/) | Создаёт объект CellsColor. |
| [Replace_String_String](./replace_string_string/) | Заменяет значение ячейки новой строкой. |
| [Replace_String_Int](./replace_string_int/) | Заменяет значение ячейки новым целым числом. |
| [Replace_String_Double](./replace_string_double/) | Заменяет значение ячейки новым числом с плавающей точкой. |
| [Replace_String_stringArray_Bool](./replace_string_stringarray_bool/) | Заменяет значение ячейки новым массивом строк. |
| [Replace_String_int32Array_Bool](./replace_string_int32array_bool/) | Заменяет значения ячеек массивом целых чисел. |
| [Replace_String_float64Array_Bool](./replace_string_float64array_bool/) | Заменяет значения ячеек массивом чисел с плавающей точкой. |
| [Replace_Bool_Object](./replace_bool_object/) | Заменяет значения ячеек новыми данными. |
| [Replace_Int_Object](./replace_int_object/) | Заменяет значения ячеек новыми данными. |
| [Replace_String_String_ReplaceOptions](./replace_string_string_replaceoptions/) | Заменяет значение ячейки новой строкой. |
| [Copy_Workbook_CopyOptions](./copy_workbook_copyoptions/) | Копирует другой объект Workbook. |
| [Copy_Workbook](./copy_workbook/) | Копирует данные из исходного объекта Workbook. |
| [Combine](./combine/) | Объединяет другой объект Workbook. |
| [GetColors](./getcolors/) | Возвращает цвета из палитры для электронной таблицы. |
| [GetStyleInPool](./getstyleinpool/) | Получает стиль из пула стилей.Все стили в книге будут собраны в пул.В ячейках хранится только простой индекс ссылки. |
| [GetCountOfStylesInPool](./getcountofstylesinpool/) | Получает количество стилей в пуле стилей. |
| [GetFonts](./getfonts/) | Получает все шрифты в пуле стилей. |
| [GetNamedStyle](./getnamedstyle/) | Получает именованный стиль из пула стилей. |
| [MergeNamedStyles](./mergenamedstyles/) | Объединяет именованные стили из другого файла Excel. |
| [ChangePalette](./changepalette/) | Изменяет палитру листа в указанном индексе. |
| [IsColorInPalette](./iscolorinpalette/) | Проверяет, находится ли цвет в палитре листа. |
| [CalculateFormula](./calculateformula/) | Вычисляет результат формул. |
| [CalculateFormula_Bool](./calculateformula_bool/) | Вычисляет результат формул. |
| [CalculateFormula_CalculationOptions](./calculateformula_calculationoptions/) | Вычисление формул в этой книге. |
| [RefreshDynamicArrayFormulas_Bool](./refreshdynamicarrayformulas_bool/) | Обновляет формулы динамических массивов (разливается в новый диапазон соседних ячеек в соответствии с текущими данными). Другие формулы в книге не будут вычисляться рекурсивно, даже если они использовались формулами динамических массивов. |
| [RefreshDynamicArrayFormulas_Bool_CalculationOptions](./refreshdynamicarrayformulas_bool_calculationoptions/) | Обновляет формулы динамических массивов (разливается в новый диапазон соседних ячеек в соответствии с текущими данными). |
| [GetDefaultStyle](./getdefaultstyle/) | Получает или задает объект Style по умолчанию книги. |
| [SetDefaultStyle](./setdefaultstyle/) | Получает или задает объект Style по умолчанию книги. |
| [GetMatchingColor](./getmatchingcolor/) | Найти наиболее подходящий Color в текущей палитре. |
| [IsDigitallySigned](./isdigitallysigned/) | Указывает, подписан ли этот лист цифровой подписью. |
| [SetEncryptionOptions](./setencryptionoptions/) | Установить параметры шифрования. |
| [Protect](./protect/) | Защищает книгу. |
| [ProtectSharedWorkbook](./protectsharedworkbook/) | Защищает общую книгу. |
| [Unprotect](./unprotect/) | Снимает защиту с книги. |
| [UnprotectSharedWorkbook](./unprotectsharedworkbook/) | Снимает защиту с общей книги. |
| [IsWorkbookProtectedWithPassword](./isworkbookprotectedwithpassword/) | Указывает, защищены ли структура или окно паролем. |
| [RemoveMacro](./removemacro/) | Удаляет VBA/макрос из этого листа. |
| [GetVbaProject](./getvbaproject/) | Получает VbaProject в листе. |
| [RemoveDigitalSignature](./removedigitalsignature/) | Удаляет цифровую подпись из этого листа. |
| [AcceptAllRevisions](./acceptallrevisions/) | Принимает все отслеживаемые изменения в книге. |
| [GetHasMacro](./gethasmacro/) | Указывает, содержит ли этот лист макрос/VBA. |
| [GetHasRevisions](./gethasrevisions/) | Определяет, есть ли в книге отслеживаемые изменения. |
| [GetFileName](./getfilename/) | Получает и задает текущее имя файла. |
| [SetFileName](./setfilename/) | Получает и задает текущее имя файла. |
| [GetDataSorter](./getdatasorter/) | Получает объект DataSorter для сортировки данных. |
| [GetThemeColor](./getthemecolor/) | Получает цвет темы. |
| [SetThemeColor](./setthemecolor/) | Устанавливает цвет темы |
| [GetTheme](./gettheme/) | Получает название темы. |
| [CustomTheme](./customtheme/) | Настраивает тему. |
| [CopyTheme](./copytheme/) | Копирует тему из другой книги. |
| [UpdateCustomFunctionDefinition](./updatecustomfunctiondefinition/) | Обновляет определение пользовательских функций. |
| [UpdateLinkedDataSource](./updatelinkeddatasource/) | Если эта книга содержит внешние ссылки на другие источники данных, Aspose.Cells попытается получить последние данные из указанных источников. |
| [GetBuiltInDocumentProperties](./getbuiltindocumentproperties/) | Возвращает коллекцию DocumentProperty, представляющую все встроенные свойства документа электронной таблицы. |
| [GetCustomDocumentProperties](./getcustomdocumentproperties/) | Возвращает коллекцию DocumentProperty, представляющую все пользовательские свойства документа электронной таблицы. |
| [GetFileFormat](./getfileformat/) | Получает и задает формат файла. |
| [SetFileFormat](./setfileformat/) | Получает и задает формат файла. |
| [GetHasCustomFunction](./gethascustomfunction/) | Определяет, используется ли в этой книге пользовательская функция, например в формулах ячеек, в определённых именах... |
| [GetInterruptMonitor](./getinterruptmonitor/) | Получает и задает монитор прерываний. |
| [SetInterruptMonitor_AbstractInterruptMonitor](./setinterruptmonitor_abstractinterruptmonitor/) | Получает и задает монитор прерываний. |
| [SetInterruptMonitor_InterruptMonitor](./setinterruptmonitor_interruptmonitor/) | Устанавливает монитор прерываний. |
| [GetContentTypeProperties](./getcontenttypeproperties/) | Получает список объектов ContentTypeProperty в книге. |
| [GetCustomXmlParts](./getcustomxmlparts/) | Представляет часть хранилища пользовательских XML‑данных (пользовательские XML‑данные внутри пакета). |
| [GetDataMashup](./getdatamashup/) | Получает данные mashup. |
| [GetRibbonXml](./getribbonxml/) | Получает и задает XML‑файл, определяющий интерфейс Ribbon. |
| [SetRibbonXml](./setribbonxml/) | Получает и задает XML‑файл, определяющий интерфейс Ribbon. |
| [GetAbsolutePath](./getabsolutepath/) | Получает и задает абсолютный путь к файлу. |
| [SetAbsolutePath](./setabsolutepath/) | Получает и задает абсолютный путь к файлу. |
| [GetDataConnections](./getdataconnections/) | Получает коллекцию ExternalConnection. |
| [ImportXml_String_String_Int_Int](./importxml_string_string_int_int/) | Импортирует/обновляет XML‑файл данных в книгу. |
| [ImportXml_Stream_String_Int_Int](./importxml_stream_string_int_int/) | Импортирует/обновляет XML‑файл данных в книгу. |
| [ExportXml_String_String](./exportxml_string_string/) | Экспортирует XML‑данные, связанные с указанной XML‑картой. |
| [ExportXml_String](./exportxml_string/) | Экспортирует XML‑данные. |
| [SetDigitalSignature](./setdigitalsignature/) | Устанавливает цифровую подпись в файл электронной таблицы (Excel2007 и новее). |
| [AddDigitalSignature](./adddigitalsignature/) | Добавляет цифровую подпись в OOXML‑файл электронной таблицы (Excel2007 и новее). |
| [GetDigitalSignature](./getdigitalsignature/) | Получает цифровую подпись из файла. |
| [RemovePersonalInformation](./removepersonalinformation/) | Удаляет личную информацию. |
| [GetDataModel](./getdatamodel/) | Получает модель данных в книге. |
| [RefreshAll](./refreshall/) | Обновить связанные фигуры, все сводные таблицы и диаграммы с источником сводных данных. |
| [Dispose](./dispose/) | Выполняет задачи, определённые приложением, связанные с освобождением, выпуском или сбросом неуправляемых ресурсов. |
