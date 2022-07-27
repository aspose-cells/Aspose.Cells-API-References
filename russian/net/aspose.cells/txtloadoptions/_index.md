---
title: TxtLoadOptions
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет параметры загрузки текстового файла.
type: docs
weight: 6110
url: /ru/net/aspose.cells/txtloadoptions/
---
## TxtLoadOptions class

Представляет параметры загрузки текстового файла.

```csharp
public class TxtLoadOptions : AbstractTextLoadOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TxtLoadOptions](txtloadoptions#constructor)() | Создает параметры для загрузки текстового файла. |
| [TxtLoadOptions](txtloadoptions#constructor_1)(LoadFormat) | Создает параметры для загрузки текстового файла. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [AutoFilter](../../aspose.cells/loadoptions/autofilter) { get; set; } | Указывает, выполняется ли автоматическая фильтрация данных при загрузке файлов. |
| [AutoFitterOptions](../../aspose.cells/loadoptions/autofitteroptions) { get; set; } | Получает и устанавливает параметры автоматической установки |
| [CheckDataValid](../../aspose.cells/loadoptions/checkdatavalid) { get; set; } | Проверить правильность данных в файле шаблона. |
| [CheckExcelRestriction](../../aspose.cells/loadoptions/checkexcelrestriction) { get; set; } | Проверять ли ограничение файла excel, когда пользователь изменяет объекты, связанные с ячейками. Например, excel не позволяет вводить строковое значение длиннее 32 КБ. имеет значение true, вы получите исключение. Если это свойство имеет значение false, мы примем введенное вами строковое значение в качестве значения ячейки, чтобы позже вы могли вывести полное строковое значение для других форматов файлов, таких как CSV. Однако, если вы установили такое значение, которое недопустимо для формата файла Excel, вам не следует сохранять книгу в формате файла Excel позже. В противном случае может возникнуть непредвиденная ошибка для сгенерированного файла Excel. |
| [ConvertDateTimeData](../../aspose.cells/abstracttextloadoptions/convertdatetimedata) { get; set; } | Получает или задает значение, указывающее, преобразуется ли строка в текстовом файле в данные даты. |
| [ConvertNumericData](../../aspose.cells/abstracttextloadoptions/convertnumericdata) { get; set; } | Получает или задает значение, указывающее, преобразуется ли строка в текстовом файле в числовые данные. |
| [CultureInfo](../../aspose.cells/loadoptions/cultureinfo) { get; set; } | Получает или задает информацию о культуре системы на момент загрузки файла. |
| [DefaultStyleSettings](../../aspose.cells/loadoptions/defaultstylesettings) { get; } | Получает настройки стиля по умолчанию для инициализации стилей рабочей книги |
| [Encoding](../../aspose.cells/abstracttextloadoptions/encoding) { get; set; } | Получает и задает кодировку по умолчанию. Применяется только для CSV-файла. |
| [ExtendToNextSheet](../../aspose.cells/txtloadoptions/extendtonextsheet) { get; set; } | Расширяет ли данные на следующий лист, когда строки или столбцы данных превышают предел. Если это свойство истинно, дополнительные данные будут расширены на следующий лист за текущим (если текущий лист является последним, будет добавлен новый лист в текущую книгу). Если для этого свойства установлено значение false, данные, превышающие лимит, будут игнорироваться. Значение по умолчанию — false; |
| [FontConfigs](../../aspose.cells/loadoptions/fontconfigs) { get; set; } | Получает и устанавливает отдельные конфигурации шрифтов. Работает только для[`Workbook`](../workbook) который использует это[`LoadOptions`](../loadoptions) для загрузки.&gt; |
| [HasFormula](../../aspose.cells/txtloadoptions/hasformula) { get; set; } | Указывает, является ли текст формулой, если он начинается с "=". |
| [HasTextQualifier](../../aspose.cells/txtloadoptions/hastextqualifier) { get; set; } | Есть ли квалификатор текста для значения ячейки. Значение по умолчанию — true. |
| [IgnoreNotPrinted](../../aspose.cells/loadoptions/ignorenotprinted) { get; set; } | Игнорировать данные, которые не печатаются, при прямой печати файла |
| [InterruptMonitor](../../aspose.cells/loadoptions/interruptmonitor) { get; set; } | Получает и устанавливает монитор прерываний. |
| [IsMultiEncoded](../../aspose.cells/txtloadoptions/ismultiencoded) { get; set; } | True означает, что файл содержит несколько кодировок. |
| [KeepPrecision](../../aspose.cells/abstracttextloadoptions/keepprecision) { get; set; } | Указывает, не анализировать ли строковое значение, если длина равна 15. |
| [KeepUnparsedData](../../aspose.cells/loadoptions/keepunparseddata) { get; set; } | Сохранять ли непроанализированные данные в памяти для книги, когда она загружается из файла шаблона. Значение по умолчанию — true. |
| [LanguageCode](../../aspose.cells/loadoptions/languagecode) { get; set; } | Получает или задает язык пользовательского интерфейса версии книги на основе CountryCode, в которой сохранен файл. |
| [LightCellsDataHandler](../../aspose.cells/loadoptions/lightcellsdatahandler) { get; set; } | Обработчик данных для обработки данных ячеек при чтении файла шаблона. |
| [LoadFilter](../../aspose.cells/loadoptions/loadfilter) { get; set; } | Фильтр для обозначения способа загрузки данных. |
| [LoadFormat](../../aspose.cells/loadoptions/loadformat) { get; } | Получает формат загрузки. |
| [LoadStyleStrategy](../../aspose.cells/abstracttextloadoptions/loadstylestrategy) { get; set; } | Указывает стратегию применения стиля для проанализированных значений при преобразовании строкового значения в число или дату и время. |
| [MemorySetting](../../aspose.cells/loadoptions/memorysetting) { get; set; } | Получает или задает параметры использования памяти. |
| [ParsingFormulaOnOpen](../../aspose.cells/loadoptions/parsingformulaonopen) { get; set; } | Указывает, выполняется ли разбор формулы при чтении файла. |
| [ParsingPivotCachedRecords](../../aspose.cells/loadoptions/parsingpivotcachedrecords) { get; set; } | Указывает, анализируются ли сводные кэшированные записи при загрузке файла. Значение по умолчанию — false. |
| [Password](../../aspose.cells/loadoptions/password) { get; set; } | Получает и устанавливает пароль книги. |
| [PreferredParsers](../../aspose.cells/txtloadoptions/preferredparsers) { get; set; } | Получает и устанавливает анализаторы предпочтительных значений для загрузки текстового файла. |
| [Region](../../aspose.cells/loadoptions/region) { get; set; } | Получает или задает региональные параметры системы на основе CountryCode на момент загрузки файла. |
| [Separator](../../aspose.cells/txtloadoptions/separator) { get; set; } | Получает и устанавливает разделитель символов текстового файла. |
| [SeparatorString](../../aspose.cells/txtloadoptions/separatorstring) { get; set; } | Получает и устанавливает строковое значение в качестве разделителя. |
| [TextQualifier](../../aspose.cells/txtloadoptions/textqualifier) { get; set; } | Указывает квалификатор текста для значений ячеек. Классификатор по умолчанию — '"'. |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells/txtloadoptions/treatconsecutivedelimitersasone) { get; set; } | Следует ли рассматривать последовательные разделители как один. |
| [TreatQuotePrefixAsValue](../../aspose.cells/txtloadoptions/treatquoteprefixasvalue) { get; set; } | Указывает, следует ли рассматривать одинарную кавычку как часть значения одной ячейки. Значение по умолчанию — true. Если оно ложно, ведущая одинарная кавычка будет удалена из значения соответствующей ячейки и[`QuotePrefix`](../style/quoteprefix) будет установлено как true для ячейки. |
| [WarningCallback](../../aspose.cells/loadoptions/warningcallback) { get; set; } | Получает или задает обратный вызов предупреждения. |

## Методы

| Имя | Описание |
| --- | --- |
| [SetPaperSize](../../aspose.cells/loadoptions/setpapersize)(PaperSizeType) | Устанавливает размер бумаги для печати по умолчанию из настроек принтера по умолчанию. |

### Смотрите также

* class [AbstractTextLoadOptions](../abstracttextloadoptions)
* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
