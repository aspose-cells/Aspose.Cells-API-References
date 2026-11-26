---
title: "Класс GridLoadOptions"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridWeb.Data.GridLoadOptions. Представляет параметры загрузки файла. Устаревший. Этот класс будет объявлен устаревшим после использования отдельной DLL публичного API Cells; вместо этого вы можете использовать Aspose.Cells.LodOptions"
type: docs
url: /ru/net/aspose.cells.gridweb.data/gridloadoptions/
---
## GridLoadOptions class

Представляет параметры загрузки файла. [Obsolete("This class will be obsoleted after stand alone dll usage of cells public api,instead you can use Aspose.Cells.LodOptions ")]

```csharp
public class GridLoadOptions : ISerializable
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GridLoadOptions](gridloadoptions/)() | Создаёт параметры загрузки файла. |

## Свойства

| Имя | Описание |
| --- | --- |
| [AutoFilter](../../aspose.cells.gridweb.data/gridloadoptions/autofilter/) { get; set; } | Указывает, следует ли автоматически фильтровать данные при загрузке файлов. |
| [CheckDataValid](../../aspose.cells.gridweb.data/gridloadoptions/checkdatavalid/) { get; set; } | Проверьте, действительны ли данные в шаблонном файле. |
| [CheckExcelRestriction](../../aspose.cells.gridweb.data/gridloadoptions/checkexcelrestriction/) { get; set; } | Проверять ли ограничения файла Excel, когда пользователь изменяет связанные с ячейками объекты. Например, Excel не позволяет вводить строковое значение длиной более 32 КБ. Когда вы вводите значение длиннее 32 КБ, например через Cell.PutValue(string), если это свойство равно true, вы получите исключение. Если свойство равно false, мы примем введённую строку как значение ячейки, чтобы позже вы могли вывести полное строковое значение в другие форматы файлов, такие как CSV. Однако, если вы задали значение, недопустимое для формата файла Excel, позже не следует сохранять рабочую книгу в формате Excel. В противном случае может возникнуть непредвиденная ошибка в сгенерированном файле Excel. |
| [IgnoreNotPrinted](../../aspose.cells.gridweb.data/gridloadoptions/ignorenotprinted/) { get; set; } | Игнорировать данные, которые не печатаются при прямой печати файла |
| [KeepUnparsedData](../../aspose.cells.gridweb.data/gridloadoptions/keepunparseddata/) { get; set; } | Определяет, сохранять ли неразобранные данные в памяти для Workbook при загрузке из шаблонного файла. По умолчанию true. |
| [OnlyAuto](../../aspose.cells.gridweb.data/gridloadoptions/onlyauto/) { get; set; } | Указывает, следует ли подгонять только те строки, высота которых не задана вручную. |
| [ParsingFormulaOnOpen](../../aspose.cells.gridweb.data/gridloadoptions/parsingformulaonopen/) { get; set; } | Указывает, следует ли разбирать формулу при чтении файла. |
| [ParsingPivotCachedRecords](../../aspose.cells.gridweb.data/gridloadoptions/parsingpivotcachedrecords/) { get; set; } | Указывает, следует ли разбирать кэшированные записи сводных таблиц при загрузке файла. Значение по умолчанию — false. |
| [Password](../../aspose.cells.gridweb.data/gridloadoptions/password/) { get; set; } | Получает и задает пароль рабочей книги. |
| [PreservePaddingSpacesInFormula](../../aspose.cells.gridweb.data/gridloadoptions/preservepaddingspacesinformula/) { get; set; } | Указывает, следует ли сохранять пробелы и переносы строк, добавленные между токенами формулы при получении и установке формул. Значение по умолчанию — false. |

### См. также

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


