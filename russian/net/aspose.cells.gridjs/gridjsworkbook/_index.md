---
title: GridJsWorkbook
second_title: Справочник по Aspose.Cells для .NET API
description: Представляет основной начальный класс для GridJs
type: docs
weight: 80
url: /ru/net/aspose.cells.gridjs/gridjsworkbook/
---
## GridJsWorkbook class

Представляет основной начальный класс для GridJs

```csharp
public class GridJsWorkbook
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [GridJsWorkbook](gridjsworkbook)() | Конструктор по умолчанию. |

## Характеристики

| Имя | Описание |
| --- | --- |
| [Settings](../../aspose.cells.gridjs/gridjsworkbook/settings) { get; set; } | Представляет параметры книги. |
| [WarningCallback](../../aspose.cells.gridjs/gridjsworkbook/warningcallback) { get; set; } | Получает или задает обратный вызов предупреждения для файла импорта. |

## Методы

| Имя | Описание |
| --- | --- |
| [CopyImageOrShape](../../aspose.cells.gridjs/gridjsworkbook/copyimageorshape)(string, string) | скопировать изображение или фигуру на лист |
| [ErrorJson](../../aspose.cells.gridjs/gridjsworkbook/errorjson)(string) | вернуть сообщение об ошибке |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson#exporttojson)() | Получить json из книги |
| [ExportToJson](../../aspose.cells.gridjs/gridjsworkbook/exporttojson#exporttojson_1)(string) | Получить json из рабочей книги |
| [ExportToJsonStringBuilder](../../aspose.cells.gridjs/gridjsworkbook/exporttojsonstringbuilder)(string) | Получить json из книги |
| [GetJsonByUid](../../aspose.cells.gridjs/gridjsworkbook/getjsonbyuid)(string, string) | получить json из кеша по uid |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_3)(string) | Импорт из файла Excel. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile)(Workbook) | Импорт из книги. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_1)(Stream, GridLoadFormat) | Импорт из потока файла excel. Должен предоставлять формат загрузки и может устанавливать GridJsWorkbook.CacheImp для реализации кэша потока |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_7)(string, string) | Импорт из файла Excel. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_4)(string, Workbook) | Импорт из файла Excel. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_2)(Stream, GridLoadFormat, string) | Импорт из потока файла excel. Должен предоставлять формат загрузки и может устанавливать GridJsWorkbook.CacheImp для реализации кэша потока |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_5)(string, Stream, GridLoadFormat) | Импорт из потока файла excel. Должен предоставлять формат загрузки и может устанавливать GridJsWorkbook.CacheImp для реализации кэша потока |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_8)(string, string, string) | Импорт из файла Excel. |
| [ImportExcelFile](../../aspose.cells.gridjs/gridjsworkbook/importexcelfile#importexcelfile_6)(string, Stream, GridLoadFormat, string) | Импорт из потока файла excel. Должен предоставлять формат загрузки и может устанавливать GridJsWorkbook.CacheImp для реализации кэша потока |
| [ImportExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/importexcelfilefromjson)(string) | Импорт файла из json |
| [InsertImage](../../aspose.cells.gridjs/gridjsworkbook/insertimage)(string, string, Stream, string) | вставить изображение на лист |
| [MergeExcelFileFromJson](../../aspose.cells.gridjs/gridjsworkbook/mergeexcelfilefromjson)(string, string) | Применить обновление стиля к файлу кеша |
| [SaveToCacheWithFileName](../../aspose.cells.gridjs/gridjsworkbook/savetocachewithfilename)(string, string, string) | Сохраняет рабочие листы в кэш, формат сохранения основан на расширении имени файла. |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile#savetoexcelfile)(Stream) | Сохраняет рабочие листы в поток на основе исходного формата файла. |
| [SaveToExcelFile](../../aspose.cells.gridjs/gridjsworkbook/savetoexcelfile#savetoexcelfile_1)(string) | Сохраняет рабочие листы по пути к файлу, если файл имеет расширение, формат сохранения основан на расширении файла. |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml#savetohtml)(Stream) | Сохраняет листы в поток, формат сохранения - html |
| [SaveToHtml](../../aspose.cells.gridjs/gridjsworkbook/savetohtml#savetohtml_1)(string) | Сохраняет рабочие листы в путь к файлу, формат сохранения - html |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf#savetopdf)(Stream) | Сохраняет рабочие листы в поток, формат сохранения - pdf |
| [SaveToPdf](../../aspose.cells.gridjs/gridjsworkbook/savetopdf#savetopdf_1)(string) | Сохраняет рабочие листы в путь к файлу, формат сохранения - pdf |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx#savetoxlsx)(Stream) | Сохраняет рабочие листы в поток, формат сохранения - xlsx |
| [SaveToXlsx](../../aspose.cells.gridjs/gridjsworkbook/savetoxlsx#savetoxlsx_1)(string) | Сохраняет рабочие листы в путь к файлу, формат сохранения xlsx |
| [SetInterruptMonitorForLoad](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforload)(GridInterruptMonitor, int) | установить InterruptMonitor для операции загрузки книги |
| [SetInterruptMonitorForSave](../../aspose.cells.gridjs/gridjsworkbook/setinterruptmonitorforsave)(GridInterruptMonitor) | установить InterruptMonitor для сохранения операции для книги |
| [UpdateCell](../../aspose.cells.gridjs/gridjsworkbook/updatecell)(string, string) | Выполнить операцию обновления |
| static [GetGridLoadFormat](../../aspose.cells.gridjs/gridjsworkbook/getgridloadformat)(string) | Получить GridLoadFormat по расширению файла |
| static [GetImageStream](../../aspose.cells.gridjs/gridjsworkbook/getimagestream)(string, string) | Получить поток изображений из книги |
| static [GetImageUrl](../../aspose.cells.gridjs/gridjsworkbook/getimageurl)(string, string, string) | Получить URL-адрес изображения |
| static [GetUidForFile](../../aspose.cells.gridjs/gridjsworkbook/getuidforfile)(string) | Сгенерировать uid для файла |

## Поля

| Имя | Описание |
| --- | --- |
| static [CacheImp](../../aspose.cells.gridjs/gridjsworkbook/cacheimp) | Пользовательская реализация для хранения кеша. Если вы хотите хранить кеш в потоковом режиме, вам нужно установить и реализовать его |
| static [CalculateEngine](../../aspose.cells.gridjs/gridjsworkbook/calculateengine) | Пользовательская реализация механизма расчета. Если вы хотите выполнить пользовательский расчет, вам необходимо установить и реализовать его |

### Смотрите также

* пространство имен [Aspose.Cells.GridJs](../../aspose.cells.gridjs)
* сборка [Aspose.Cells.GridJs](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.GridJs.dll -->
