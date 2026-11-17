---
title: "Класс TxtLoadOptions"
linktitle: "TxtLoadOptions"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "Класс TxtLoadOptions. Инкапсулирует объект, представляющий txtloadoptions в Go."
type: docs
weight: 200
url: /ru/go-cpp/txtloadoptions/
---

## TxtLoadOptions class

Представляет параметры загрузки текстового файла.

```go

type TxtLoadOptions struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewTxtLoadOptions](./newtxtloadoptions/) | Создаёт параметры для загрузки текстового файла. |
| [NewTxtLoadOptions_LoadFormat](./newtxtloadoptions_loadformat/) | Создаёт параметры для загрузки текстового файла. |
| [NewTxtLoadOptions_AbstractTextLoadOptions](./newtxtloadoptions_abstracttextloadoptions/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetSeparator](./getseparator/) | Получает и задаёт разделитель символов текстового файла. |
| [SetSeparator](./setseparator/) | Получает и задаёт разделитель символов текстового файла. |
| [GetSeparatorString](./getseparatorstring/) | Получает и задаёт строковое значение в качестве разделителя. |
| [SetSeparatorString](./setseparatorstring/) | Получает и задаёт строковое значение в качестве разделителя. |
| [IsMultiEncoded](./ismultiencoded/) | True означает, что файл содержит несколько кодировок. |
| [SetIsMultiEncoded](./setismultiencoded/) | True означает, что файл содержит несколько кодировок. |
| [GetHasFormula](./gethasformula/) | Указывает, является ли текст формулой, если он начинается с "=","Получает и задаёт кодировку по умолчанию. Применяется только для файлов csv. |
| [SetHasFormula](./sethasformula/) | Указывает, является ли текст формулой, если он начинается с "=","Получает и задаёт кодировку по умолчанию. Применяется только для файлов csv. |
| [GetHasTextQualifier](./gethastextqualifier/) | Определяет, есть ли текстовый квалификатор для значения ячейки. По умолчанию true. |
| [SetHasTextQualifier](./sethastextqualifier/) | Определяет, есть ли текстовый квалификатор для значения ячейки. По умолчанию true. |
| [GetTextQualifier](./gettextqualifier/) | Указывает текстовый квалификатор для значений ячеек. Квалификатор по умолчанию — \". |
| [SetTextQualifier](./settextqualifier/) | Указывает текстовый квалификатор для значений ячеек. Квалификатор по умолчанию — \". |
| [GetTreatConsecutiveDelimitersAsOne](./gettreatconsecutivedelimitersasone/) | Определяет, следует ли рассматривать последовательные разделители как один. |
| [SetTreatConsecutiveDelimitersAsOne](./settreatconsecutivedelimitersasone/) | Определяет, следует ли рассматривать последовательные разделители как один. |
| [GetTreatQuotePrefixAsValue](./gettreatquoteprefixasvalue/) | Указывает, следует ли учитывать начальный одинарный апостроф как часть значения ячейки. По умолчанию true. Если false, начальный одинарный апостроф будет удалён из соответствующего значения ячейки, и для ячейки будет установлен Style.QuotePrefix в значение true. |
| [SetTreatQuotePrefixAsValue](./settreatquoteprefixasvalue/) | Указывает, следует ли учитывать начальный одинарный апостроф как часть значения ячейки. По умолчанию true. Если false, начальный одинарный апостроф будет удалён из соответствующего значения ячейки, и для ячейки будет установлен Style.QuotePrefix в значение true. |
| [GetExtendToNextSheet](./getextendtonextsheet/) | Определяет, следует ли переносить данные на следующий лист, когда количество строк или столбцов превышает предел. По умолчанию false. |
| [SetExtendToNextSheet](./setextendtonextsheet/) | Определяет, следует ли переносить данные на следующий лист, когда количество строк или столбцов превышает предел. По умолчанию false. |
| [GetHeaderRowsCount](./getheaderrowscount/) | Количество строк заголовка, которые нужно повторять для расширенных листов. |
| [SetHeaderRowsCount](./setheaderrowscount/) | Количество строк заголовка, которые нужно повторять для расширенных листов. |
| [GetHeaderColumnsCount](./getheadercolumnscount/) | Количество столбцов заголовка, которые должны повторяться для расширенных листов. |
| [SetHeaderColumnsCount](./setheadercolumnscount/) | Количество столбцов заголовка, которые должны повторяться для расширенных листов. |
| [GetMaxRowCount](./getmaxrowcount/) | Максимальное количество строк, которые могут быть импортированы для одного листа. |
| [SetMaxRowCount](./setmaxrowcount/) | Максимальное количество строк, которые могут быть импортированы для одного листа. |
| [GetMaxColumnCount](./getmaxcolumncount/) | Максимальное количество столбцов, которые могут быть импортированы для одного листа. |
| [SetMaxColumnCount](./setmaxcolumncount/) | Максимальное количество столбцов, которые могут быть импортированы для одного листа. |
| [GetEncoding](./getencoding/) | Указывает стратегию применения стиля к разобранным значениям при преобразовании строкового значения в число или дату/время. |
| [SetEncoding](./setencoding/) | Указывает стратегию применения стиля к разобранным значениям при преобразовании строкового значения в число или дату/время. |
| [GetLoadStyleStrategy](./getloadstylestrategy/) | Получает или задаёт значение, указывающее, преобразуется ли строка в текстовом файле в числовые данные. Значение по умолчанию — true. |
| [SetLoadStyleStrategy](./setloadstylestrategy/) | Получает или задаёт значение, указывающее, преобразуется ли строка в текстовом файле в числовые данные. Значение по умолчанию — true. |
| [GetConvertNumericData](./getconvertnumericdata/) | Получает или задаёт значение, указывающее, преобразуется ли строка в текстовом файле в дату. Значение по умолчанию — true. |
| [SetConvertNumericData](./setconvertnumericdata/) | Получает или задаёт значение, указывающее, преобразуется ли строка в текстовом файле в дату. Значение по умолчанию — true. |
| [GetConvertDateTimeData](./getconvertdatetimedata/) | Указывает, не разбирать ли строковое значение, если его длина равна 15. |
| [SetConvertDateTimeData](./setconvertdatetimedata/) | Указывает, не разбирать ли строковое значение, если его длина равна 15. |
| [GetKeepPrecision](./getkeepprecision/) | Указывает, не разбирать ли строковое значение, если длина равна 15. |
| [SetKeepPrecision](./setkeepprecision/) | Указывает, не разбирать ли строковое значение, если длина равна 15. |
| [GetLoadFormat](./getloadformat/) | Получает формат загрузки. |
| [GetPassword](./getpassword/) | Получает и задает пароль рабочей книги. |
| [SetPassword](./setpassword/) | Получает и задает пароль рабочей книги. |
| [GetParsingFormulaOnOpen](./getparsingformulaonopen/) | Указывает, выполнять ли разбор формулы при чтении файла. |
| [SetParsingFormulaOnOpen](./setparsingformulaonopen/) | Указывает, выполнять ли разбор формулы при чтении файла. |
| [GetParsingPivotCachedRecords](./getparsingpivotcachedrecords/) | Указывает, выполнять ли разбор кэшированных записей сводных таблиц при загрузке файла. Значение по умолчанию — false. |
| [SetParsingPivotCachedRecords](./setparsingpivotcachedrecords/) | Указывает, выполнять ли разбор кэшированных записей сводных таблиц при загрузке файла. Значение по умолчанию — false. |
| [SetPaperSize](./setpapersize/) | Устанавливает размер бумаги по умолчанию для печати из настроек принтера по умолчанию. |
| [GetLanguageCode](./getlanguagecode/) | Получает или задает язык пользовательского интерфейса версии Workbook на основе CountryCode, в которой был сохранён файл. |
| [SetLanguageCode](./setlanguagecode/) | Получает или задает язык пользовательского интерфейса версии Workbook на основе CountryCode, в которой был сохранён файл. |
| [GetRegion](./getregion/) | Получает или задает региональные настройки, используемые для загружаемой рабочей книги. |
| [SetRegion](./setregion/) | Получает или задает региональные настройки, используемые для загружаемой рабочей книги. |
| [GetDefaultStyleSettings](./getdefaultstylesettings/) | Получает настройки стиля по умолчанию для инициализации стилей рабочей книги. |
| [GetInterruptMonitor](./getinterruptmonitor/) | Получает и задает монитор прерываний. |
| [SetInterruptMonitor](./setinterruptmonitor/) | Получает и задает монитор прерываний. |
| [GetIgnoreNotPrinted](./getignorenotprinted/) | Игнорировать данные, которые не печатаются при прямой печати файла. |
| [SetIgnoreNotPrinted](./setignorenotprinted/) | Игнорировать данные, которые не печатаются при прямой печати файла. |
| [GetCheckDataValid](./getcheckdatavalid/) | Проверять, являются ли данные действительными в шаблонном файле. |
| [SetCheckDataValid](./setcheckdatavalid/) | Проверять, являются ли данные действительными в шаблонном файле. |
| [GetCheckExcelRestriction](./getcheckexcelrestriction/) | Определяет, проверять ли ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Если вы вводите значение длиной более 32 КБ, например с помощью Cell.PutValue(string), и это свойство установлено в true, будет выброшено исключение. Если свойство установлено в false, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, которое недействительно для формата Excel, не следует сохранять рабочую книгу в формате Excel позже. В противном случае может возникнуть непредвиденная ошибка в сгенерированном файле Excel. |
| [SetCheckExcelRestriction](./setcheckexcelrestriction/) | Определяет, проверять ли ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Если вы вводите значение длиной более 32 КБ, например с помощью Cell.PutValue(string), и это свойство установлено в true, будет выброшено исключение. Если свойство установлено в false, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, которое недействительно для формата Excel, не следует сохранять рабочую книгу в формате Excel позже. В противном случае может возникнуть непредвиденная ошибка в сгенерированном файле Excel. |
| [GetKeepUnparsedData](./getkeepunparseddata/) | Определяет, сохранять ли неразобранные данные в памяти для Workbook при загрузке из шаблонного файла. По умолчанию — true. |
| [SetKeepUnparsedData](./setkeepunparseddata/) | Определяет, сохранять ли неразобранные данные в памяти для Workbook при загрузке из шаблонного файла. По умолчанию — true. |
| [GetLoadFilter](./getloadfilter/) | Фильтр, указывающий, как загружать данные. |
| [SetLoadFilter](./setloadfilter/) | Фильтр, указывающий, как загружать данные. |
| [GetMemorySetting](./getmemorysetting/) | Получает или задает режим памяти для загруженной рабочей книги. |
| [SetMemorySetting](./setmemorysetting/) | Получает или задает режим памяти для загруженной рабочей книги. |
| [GetAutoFitterOptions](./getautofitteroptions/) | Получает и задает параметры автоподгонки. |
| [SetAutoFitterOptions](./setautofitteroptions/) | Получает и задает параметры автоподгонки. |
| [GetAutoFilter](./getautofilter/) | Указывает, выполнять ли автоматическую фильтрацию данных при загрузке файлов. |
| [SetAutoFilter](./setautofilter/) | Указывает, выполнять ли автоматическую фильтрацию данных при загрузке файлов. |
| [GetFontConfigs](./getfontconfigs/) | Получает и задает отдельные конфигурации шрифтов. Работает только с Workbook, который загружается с помощью этих LoadOptions. |
| [SetFontConfigs](./setfontconfigs/) | Получает и задает отдельные конфигурации шрифтов. Работает только с Workbook, который загружается с помощью этих LoadOptions. |
| [GetIgnoreUselessShapes](./getignoreuselessshapes/) | Указывает, игнорировать ли бесполезные фигуры. |
| [SetIgnoreUselessShapes](./setignoreuselessshapes/) | Указывает, игнорировать ли бесполезные фигуры. |
| [GetPreservePaddingSpacesInFormula](./getpreservepaddingspacesinformula/) | Указывает, сохранять ли пробелы и разрывы строк, вставленные между токенами формулы при получении и установке формул. Значение по умолчанию — false. |
| [SetPreservePaddingSpacesInFormula](./setpreservepaddingspacesinformula/) | Указывает, сохранять ли пробелы и разрывы строк, вставленные между токенами формулы при получении и установке формул. Значение по умолчанию — false. |
