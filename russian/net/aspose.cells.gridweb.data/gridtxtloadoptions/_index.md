---
title: "Класс GridTxtLoadOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridWeb.Data.GridTxtLoadOptions. Представляет параметры загрузки текстового файла"
type: docs
url: /ru/net/aspose.cells.gridweb.data/gridtxtloadoptions/
---
## GridTxtLoadOptions class

Представляет параметры загрузки текстового файла.

```csharp
[Obsolete("This class will be obsoleted after stand alone dll usage of cells public api,instead you can use Aspose.Cells.TxtLoadOptions ")]
public class GridTxtLoadOptions : GridLoadOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GridTxtLoadOptions](gridtxtloadoptions/)() | Создаёт параметры для загрузки текстового файла. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AutoFilter](../../aspose.cells.gridweb.data/gridloadoptions/autofilter/) { get; set; } | Указывает, следует ли автоматически фильтровать данные при загрузке файлов.(Наследовано от [`GridLoadOptions`](../gridloadoptions/).) |
| [CheckDataValid](../../aspose.cells.gridweb.data/gridloadoptions/checkdatavalid/) { get; set; } | Проверьте, являются ли данные действительными в файле шаблона.(Наследовано от [`GridLoadOptions`](../gridloadoptions/).) |
| [CheckExcelRestriction](../../aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/) { get; set; } | Указывает, проверять ли ограничения файла Excel при изменении пользователем связанных объектов ячеек. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Когда вы вводите значение длиной более 32 КБ, например с помощью Cell.PutValue(string), если это свойство истинно, вы получите исключение. Если свойство ложно, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, недопустимое для формата файла Excel, не следует позже сохранять книгу в формате Excel. В противном случае могут возникнуть непредвиденные ошибки в сгенерированном файле Excel.(Наследовано от [`GridLoadOptions`](../gridloadoptions/).) |
| [ConvertDateTimeData](../../aspose.cells.gridweb.data/gridtxtloadoptions/convertdatetimedata/) { get; set; } | Получает или задает значение, указывающее, преобразуется ли строка в текстовом файле в данные даты. |
| [ConvertNumericData](../../aspose.cells.gridweb.data/gridtxtloadoptions/convertnumericdata/) { get; set; } | Получает или задает значение, указывающее, преобразуется ли строка в текстовом файле в числовые данные. |
| [Encoding](../../aspose.cells.gridweb.data/gridtxtloadoptions/encoding/) { get; set; } | Получает и задает кодировку по умолчанию. Применяется только к файлам csv. |
| [ExtendToNextSheet](../../aspose.cells.gridweb.data/gridtxtloadoptions/extendtonextsheet/) { get; set; } | Указывает, расширять ли данные на следующий лист, когда строки или столбцы данных превышают ограничение. Если это свойство истинно, дополнительные данные будут перенесены на следующий лист позади текущего (если текущий лист последний, будет добавлен новый лист в текущую книгу). Если свойство ложно, данные, превышающие ограничение, будут игнорироваться. По умолчанию — false; |
| [HasFormula](../../aspose.cells.gridweb.data/gridtxtloadoptions/hasformula/) { get; set; } | Указывает, является ли текст формулой, если он начинается с "=". |
| [HasTextQualifier](../../aspose.cells.gridweb.data/gridtxtloadoptions/hastextqualifier/) { get; set; } | Определяет, есть ли текстовый квалификатор для значения ячейки. По умолчанию true. |
| [IgnoreNotPrinted](../../aspose.cells.gridweb.data/gridloadoptions/ignorenotprinted/) { get; set; } | Игнорировать данные, которые не печатаются при прямой печати файла(Наследовано от [`GridLoadOptions`](../gridloadoptions/).) |
| [IsMultiEncoded](../../aspose.cells.gridweb.data/gridtxtloadoptions/ismultiencoded/) { get; set; } | True означает, что файл содержит несколько кодировок. |
| [KeepPrecision](../../aspose.cells.gridweb.data/gridtxtloadoptions/keepprecision/) { get; set; } | Указывает, не разбирать строковое значение, если его длина равна 15. |
| [KeepUnparsedData](../../aspose.cells.gridweb.data/gridloadoptions/keepunparseddata/) { get; set; } | Указывает, сохранять ли неразобранные данные в памяти для Workbook при загрузке из файла шаблона. По умолчанию — true.(Наследовано от [`GridLoadOptions`](../gridloadoptions/).) |
| [OnlyAuto](../../aspose.cells.gridweb.data/gridloadoptions/onlyauto/) { get; set; } | Указывает, подгонять ли только строки, высота которых не настроена вручную.(Наследовано от [`GridLoadOptions`](../gridloadoptions/).) |
| [ParsingFormulaOnOpen](../../aspose.cells.gridweb.data/gridloadoptions/parsingformulaonopen/) { get; set; } | Указывает, выполнять ли разбор формулы при чтении файла.(Наследовано от [`GridLoadOptions`](../gridloadoptions/).) |
| [ParsingPivotCachedRecords](../../aspose.cells.gridweb.data/gridloadoptions/parsingpivotcachedrecords/) { get; set; } | Указывает, выполнять ли разбор кэшированных записей сводной таблицы при загрузке файла. Значение по умолчанию — false.(Наследовано от [`GridLoadOptions`](../gridloadoptions/).) |
| [Password](../../aspose.cells.gridweb.data/gridloadoptions/password/) { get; set; } | Получает и задает пароль книги.(Наследовано от [`GridLoadOptions`](../gridloadoptions/).) |
| [PreservePaddingSpacesInFormula](../../aspose.cells.gridweb.data/gridloadoptions/preservepaddingspacesinformula/) { get; set; } | Указывает, сохранять ли пробелы и разрывы строк, вставленные между токенами формулы при получении и установке формул. Значение по умолчанию — false.(Наследовано от [`GridLoadOptions`](../gridloadoptions/).) |
| [Separator](../../aspose.cells.gridweb.data/gridtxtloadoptions/separator/) { get; set; } | Получает и задаёт символьный разделитель текстового файла. |
| [SeparatorString](../../aspose.cells.gridweb.data/gridtxtloadoptions/separatorstring/) { get; set; } | Получает и задаёт строковое значение в качестве разделителя. |
| [TextQualifier](../../aspose.cells.gridweb.data/gridtxtloadoptions/textqualifier/) { get; set; } | Указывает текстовый квалификатор для значений ячеек. Квалификатор по умолчанию — '"'. |
| [TreatConsecutiveDelimitersAsOne](../../aspose.cells.gridweb.data/gridtxtloadoptions/treatconsecutivedelimitersasone/) { get; set; } | Определяет, следует ли рассматривать последовательные разделители как один. |
| [TreatQuotePrefixAsValue](../../aspose.cells.gridweb.data/gridtxtloadoptions/treatquoteprefixasvalue/) { get; set; } | Указывает, следует ли считать начальный одинарный апостроф частью значения ячейки. По умолчанию — true. Если значение ложно, начальный одинарный апостроф будет удалён из соответствующего значения ячейки, и для ячейки будет установлен [`QuotePrefix`](../../aspose.cells.gridweb/gridtableitemstyle/quoteprefix/) в значение true. |

### См. также

* class [GridLoadOptions](../gridloadoptions/)
* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


