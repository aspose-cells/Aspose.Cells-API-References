---
title: TxtSaveOptions
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет параметры сохранения для CSV/разделителей табуляции/другого текстового формата.
type: docs
weight: 6130
url: /ru/net/aspose.cells/txtsaveoptions/
---
## TxtSaveOptions class

Представляет параметры сохранения для CSV/разделителей табуляции/другого текстового формата.

```csharp
public class TxtSaveOptions : SaveOptions
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [TxtSaveOptions](txtsaveoptions#constructor)() | Создает параметры сохранения текстового файла. |
| [TxtSaveOptions](txtsaveoptions#constructor_1)(SaveFormat) | Создает параметры сохранения текстового файла. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder) { get; set; } | Папка с кэшированными файлами используется для хранения больших данных. |
| [ClearData](../../aspose.cells/saveoptions/cleardata) { get; set; } | Сделайте рабочую книгу пустой после сохранения файла. |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory) { get; set; } | Если true и каталог не существует, каталог будет автоматически создан перед сохранением файла. |
| [Encoding](../../aspose.cells/txtsaveoptions/encoding) { get; set; } | Получает и устанавливает кодировку по умолчанию. |
| [ExportAllSheets](../../aspose.cells/txtsaveoptions/exportallsheets) { get; set; } | Указывает, экспортируются ли все листы в текстовый файл. Если значение равно false, экспортируется только активный лист, как в MS Excel. |
| [ExportArea](../../aspose.cells/txtsaveoptions/exportarea) { get; set; } | Диапазон экспортируемых ячеек. |
| [ExportQuotePrefix](../../aspose.cells/txtsaveoptions/exportquoteprefix) { get; set; } | Указывает, следует ли экспортировать знак одинарной кавычки как часть значения одного cell , когда[`QuotePrefix`](../style/quoteprefix) верно для него. По умолчанию false. |
| [FormatStrategy](../../aspose.cells/txtsaveoptions/formatstrategy) { get; set; } | Получает и задает стратегию форматирования при экспорте значения ячейки в виде строки. |
| [KeepSeparatorsForBlankRow](../../aspose.cells/txtsaveoptions/keepseparatorsforblankrow) { get; set; } | Указывает, следует ли выводить разделители для пустой строки. Значение по умолчанию — false, поэтому по умолчанию содержимое пустой строки будет пустым. |
| [LightCellsDataProvider](../../aspose.cells/txtsaveoptions/lightcellsdataprovider) { get; set; } | Поставщик данных для предоставления данных ячеек для сохранения книги в облегченном режиме. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas) { get; set; } | Указывает, объединяются ли области условного форматирования и проверки перед сохранением файла. |
| [QuoteType](../../aspose.cells/txtsaveoptions/quotetype) { get; set; } | Получает или задает, как заключать в кавычки значения в экспортированном текстовом файле. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache) { get; set; } | Указывает, нужно ли обновлять кэш диаграммы data |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat) { get; } | Получает формат файла сохранения. |
| [Separator](../../aspose.cells/txtsaveoptions/separator) { get; set; } | Получает и устанавливает символьный разделитель текстового файла. |
| [SeparatorString](../../aspose.cells/txtsaveoptions/separatorstring) { get; set; } | Получает и устанавливает строковое значение в качестве разделителя. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames) { get; set; } | Указывает, выполняется ли сортировка внешних определенных имен перед сохранением файла. |
| [SortNames](../../aspose.cells/saveoptions/sortnames) { get; set; } | Указывает, выполняется ли сортировка определенных имен перед сохранением файла. |
| [TrimLeadingBlankRowAndColumn](../../aspose.cells/txtsaveoptions/trimleadingblankrowandcolumn) { get; set; } | Указывает, следует ли обрезать начальные пустые строки и столбцы, как это делает MS Excel. Значение по умолчанию — true. |
| [TrimTailingBlankCells](../../aspose.cells/txtsaveoptions/trimtailingblankcells) { get; set; } | Указывает, следует ли обрезать хвостовые пустые ячейки в одной строке. По умолчанию false. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart) { get; set; } | Указывает, обновляются ли настройки Smart Art. Значение по умолчанию — false. |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas) { get; set; } | Указывает, следует ли проверять объединенные ячейки перед сохранением файла. |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback) { get; set; } | Получает или задает обратный вызов предупреждения. |

### Смотрите также

* class [SaveOptions](../saveoptions)
* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
