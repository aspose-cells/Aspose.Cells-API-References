---
title: "Класс WebWorksheets"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridWeb.Data.WebWorksheets."
type: docs
url: /ru/net/aspose.cells.gridweb.data/webworksheets/
---
## WebWorksheets class

```csharp
[Obsolete("This class is obsolete; use  GridWorksheetCollection instead")]
public class WebWorksheets : ICollection, ISerializable
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [WebWorksheets](webworksheets/)(MainWeb, GridWorksheetCollection) |  |

## Свойства

| Имя | Описание |
| --- | --- |
| [ActiveSheet](../../aspose.cells.gridweb.data/webworksheets/activesheet/) { get; } |  |
| [ActiveSheetIndex](../../aspose.cells.gridweb.data/webworksheets/activesheetindex/) { get; set; } |  |
| [Count](../../aspose.cells.gridweb.data/webworksheets/count/) { get; } |  |
| [DefaultFontName](../../aspose.cells.gridweb.data/webworksheets/defaultfontname/) { get; set; } |  |
| [DefaultFontSize](../../aspose.cells.gridweb.data/webworksheets/defaultfontsize/) { get; set; } |  |
| [IsFixedSize](../../aspose.cells.gridweb.data/webworksheets/isfixedsize/) { get; } | Возвращает значение, указывающее, имеет ли коллекция фиксированный размер. |
| [IsReadOnly](../../aspose.cells.gridweb.data/webworksheets/isreadonly/) { get; } | Возвращает значение, указывающее, является ли IList только для чтения. |
| [IsSynchronized](../../aspose.cells.gridweb.data/webworksheets/issynchronized/) { get; } | Возвращает значение, указывающее, синхронизирован ли доступ к ICollection (потокобезопасен). |
| [Item](../../aspose.cells.gridweb.data/webworksheets/item/) { get; } | Возвращает элемент Worksheet по указанному индексу. (2 индексатора) |
| [PivotCaches](../../aspose.cells.gridweb.data/webworksheets/pivotcaches/) { get; } | Возвращает объект коллекции PivotCache |
| [PivotTables](../../aspose.cells.gridweb.data/webworksheets/pivottables/) { get; } | Возвращает объект коллекции pivotTable. |
| [SyncRoot](../../aspose.cells.gridweb.data/webworksheets/syncroot/) { get; } | Возвращает объект, который можно использовать для синхронизации доступа к ICollection. |

## Методы

| Имя | Описание |
| --- | --- |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add)() | Добавляет лист в коллекцию. |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add_1)(object) | Добавляет объект листа. |
| [Add](../../aspose.cells.gridweb.data/webworksheets/add/#add_2)(string) | Добавляет лист в коллекцию. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy_1)(int) | Добавляет лист в коллекцию и копирует данные из существующего листа. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy_2)(string) | Добавляет лист в коллекцию и копирует данные из существующего листа. |
| [AddCopy](../../aspose.cells.gridweb.data/webworksheets/addcopy/#addcopy)(WebWorksheet) | Добавляет лист в коллекцию и копирует данные из существующего листа. |
| [Clear](../../aspose.cells.gridweb.data/webworksheets/clear/)() | Очищает все листы. |
| [Contains](../../aspose.cells.gridweb.data/webworksheets/contains/)(object) | Указывает, содержит ли коллекция лист. |
| [CopyTo](../../aspose.cells.gridweb.data/webworksheets/copyto/)(Array, int) | Копирует содержимое в массив. |
| [GetEnumerator](../../aspose.cells.gridweb.data/webworksheets/getenumerator/)() |  |
| [ImportDataView](../../aspose.cells.gridweb.data/webworksheets/importdataview/#importdataview)(DataView, TableItemStyle, TableItemStyle) | Импортирует из DataView. Автоматически создает лист с именем таблицы DataView. |
| [ImportDataView](../../aspose.cells.gridweb.data/webworksheets/importdataview/#importdataview_1)(DataView, TableItemStyle, TableItemStyle, string, int, int) | Импортирует из DataView в указанный лист и позицию. |
| [ImportExcelFile](../../aspose.cells.gridweb.data/webworksheets/importexcelfile/#importexcelfile)(Stream) | Импортирует из потока Excel‑файла, включая поток с диска или поток памяти. |
| [ImportExcelFile](../../aspose.cells.gridweb.data/webworksheets/importexcelfile/#importexcelfile_1)(string) | Импортирует из Excel‑файла. |
| [IndexOf](../../aspose.cells.gridweb.data/webworksheets/indexof/)(object) | Возвращает индекс листа. |
| [Insert](../../aspose.cells.gridweb.data/webworksheets/insert/)(int, string) | Вставляет лист в указанный индекс. |
| [LoadCSVFile](../../aspose.cells.gridweb.data/webworksheets/loadcsvfile/#loadcsvfile)(Stream) | Загружает данные из потока CSV‑файла. |
| [LoadCSVFile](../../aspose.cells.gridweb.data/webworksheets/loadcsvfile/#loadcsvfile_1)(string) | Загружает данные из CSV‑файла. |
| [LoadHTMLFile](../../aspose.cells.gridweb.data/webworksheets/loadhtmlfile/#loadhtmlfile)(Stream) | Загружает данные из потока HTML‑файла. |
| [LoadHTMLFile](../../aspose.cells.gridweb.data/webworksheets/loadhtmlfile/#loadhtmlfile_1)(string) | Загружает данные из HTML‑файла. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/loadspreadsheetmlfile/#loadspreadsheetmlfile)(Stream) | Загружает данные из потока файла SpreadSheetML. |
| [LoadSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/loadspreadsheetmlfile/#loadspreadsheetmlfile_1)(string) | Загружает данные из файла SpreadSheetML. |
| [Remove](../../aspose.cells.gridweb.data/webworksheets/remove/)(object) | Удаляет лист. |
| [RemoveAt](../../aspose.cells.gridweb.data/webworksheets/removeat/#removeat)(int) | Удаляет лист по индексу. |
| [RemoveAt](../../aspose.cells.gridweb.data/webworksheets/removeat/#removeat_1)(string) | Удаляет элемент по указанному имени. |
| [RunAllFormulas](../../aspose.cells.gridweb.data/webworksheets/runallformulas/)() | Выполняет формулы всех ячеек. |
| [SaveCSVFile](../../aspose.cells.gridweb.data/webworksheets/savecsvfile/#savecsvfile)(Stream) | Сохраняет данные в поток CSV‑файла. |
| [SaveCSVFile](../../aspose.cells.gridweb.data/webworksheets/savecsvfile/#savecsvfile_1)(string) | Сохраняет данные в CSV‑файл. |
| [SaveHTMLFile](../../aspose.cells.gridweb.data/webworksheets/savehtmlfile/#savehtmlfile)(Stream) | Сохраняет данные в поток HTML‑файла. |
| [SaveHTMLFile](../../aspose.cells.gridweb.data/webworksheets/savehtmlfile/#savehtmlfile_1)(string) | Сохраняет данные в HTML‑файл. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/savespreadsheetmlfile/#savespreadsheetmlfile)(Stream) | Сохраняет данные в поток файла SpreadSheetML. |
| [SaveSpreadSheetMLFile](../../aspose.cells.gridweb.data/webworksheets/savespreadsheetmlfile/#savespreadsheetmlfile_1)(string) | Сохраняет данные в файл SpreadSheetML. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile)(Stream) | Сохраняет листы в поток Excel‑файла, включая дисковый IO‑поток или поток в памяти. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_2)(string) | Сохраняет листы в Excel‑файл в формате Excel 2003. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_1)(Stream, GridSaveFormat) | Сохраняет листы в Excel‑файл. |
| [SaveToExcelFile](../../aspose.cells.gridweb.data/webworksheets/savetoexcelfile/#savetoexcelfile_3)(string, GridSaveFormat) | Сохраняет листы в Excel‑файл. |

### Примечания

ПРИМЕЧАНИЕ: Этот класс теперь устарел. пожалуйста, используйте GridWorksheetCollection вместо него. Этот класс будет удалён через 6 месяцев после августа 2014 года. Aspose извиняется за любые неудобства, которые вы могли испытать.

### См. также

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


