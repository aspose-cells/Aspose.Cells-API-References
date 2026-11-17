---
title: "XmlLoadOptions Класс"
linktitle: "XmlLoadOptions"
second_title: "Справочник API Aspose.Cells for Go через C++"
description: "XmlLoadOptions класс. Инкапсулирует объект, представляющий xmlloadoptions в Go."
type: docs
weight: 200
url: /ru/go-cpp/xmlloadoptions/
---

## XmlLoadOptions class

Представляет параметры загрузки xml.

```go

type XmlLoadOptions struct  {
	ptr unsafe.Pointer
}

```
## Конструкторы

| Метод | Описание |
| --- | --- |
| [NewXmlLoadOptions](./newxmlloadoptions/) | Представляет параметры загрузки XML‑файла. |
| [NewXmlLoadOptions_LoadFormat](./newxmlloadoptions_loadformat/) | Представляет параметры загрузки XML‑файла. |
| [NewXmlLoadOptions_LoadOptions](./newxmlloadoptions_loadoptions/) | Создаётся из родительского объекта. |

## Методы

| Метод | Описание |
| --- | --- |
| [IsNull](./isnull/) | Проверяет, является ли объект реализации nullptr. |
| [GetStartCell](./getstartcell/) | Получает и задает начальную ячейку. |
| [SetStartCell](./setstartcell/) | Получает и задает начальную ячейку. |
| [IsXmlMap](./isxmlmap/) | Указывает, выполнять ли сопоставление XML с Excel. Значение по умолчанию — false. |
| [SetIsXmlMap](./setisxmlmap/) | Указывает, выполнять ли сопоставление XML с Excel. Значение по умолчанию — false. |
| [GetContainsMultipleWorksheets](./getcontainsmultipleworksheets/) | Указывает, импортировать ли XML как несколько листов. |
| [SetContainsMultipleWorksheets](./setcontainsmultipleworksheets/) | Указывает, импортировать ли XML как несколько листов. |
| [GetConvertNumericOrDate](./getconvertnumericordate/) | Указывает, преобразовывать ли значение в XML‑файле в числовое или дату. |
| [SetConvertNumericOrDate](./setconvertnumericordate/) | Указывает, преобразовывать ли значение в XML‑файле в числовое или дату. |
| [Get_NumberFormat](./get_numberformat/) | Получает и задает формат числового значения. |
| [SetNumberFormat](./setnumberformat/) | Получает и задает формат числового значения. |
| [Get_DateFormat](./get_dateformat/) | Получает и задает формат датового значения. |
| [SetDateFormat](./setdateformat/) | Получает и задает формат датового значения. |
| [GetIgnoreRootAttributes](./getignorerootattributes/) | Указывает, игнорировать ли атрибуты корневого элемента. |
| [SetIgnoreRootAttributes](./setignorerootattributes/) | Указывает, игнорировать ли атрибуты корневого элемента. |
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
