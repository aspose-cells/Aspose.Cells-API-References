---
title: "Класс RowFilterSettings"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.GridWeb.Data.RowFilterSettings. Краткое описание для RowFilter."
type: docs
url: /ru/net/aspose.cells.gridweb.data/rowfiltersettings/
---
## RowFilterSettings class

Краткое описание для RowFilter.

```csharp
[Obsolete("This class is obsolete; use  GridWorksheet.AddAutoFilter/FilterString for autofilter /custom filter settings")]
public class RowFilterSettings : IComparer, ISerializable
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Criteria](../../aspose.cells.gridweb.data/rowfiltersettings/criteria/) { get; set; } | Строка критериев фильтра. |
| [EnableAutoFilter](../../aspose.cells.gridweb.data/rowfiltersettings/enableautofilter/) { get; set; } | Включает автоматическую фильтрацию. HeaderRow будет отображать выпадающие кнопки, позволяющие пользователю выбрать значение столбца для фильтрации. |
| [EndColumn](../../aspose.cells.gridweb.data/rowfiltersettings/endcolumn/) { get; set; } | Номер конечной строки диапазона фильтра. Если это значение установлено в -1, используется номер последней строки листа. |
| [HeaderRow](../../aspose.cells.gridweb.data/rowfiltersettings/headerrow/) { get; set; } | Номер строки заголовка, в которой будут отображаться выпадающие кнопки фильтра. |
| [StartColumn](../../aspose.cells.gridweb.data/rowfiltersettings/startcolumn/) { get; set; } | Номер начальной строки диапазона фильтра. |

## Методы

| Имя | Описание |
| --- | --- |
| [BuildAutoFilterCriteria](../../aspose.cells.gridweb.data/rowfiltersettings/buildautofiltercriteria/)() | Создает строку критериев из настроек автоматического фильтра. |
| [ClearFilter](../../aspose.cells.gridweb.data/rowfiltersettings/clearfilter/)() | Очищает все настройки фильтра и отображает все строки. |
| [CustomFilter](../../aspose.cells.gridweb.data/rowfiltersettings/customfilter/)(int, ICustomFilter) | Указывает пользовательский фильтр. |
| [FilterRows](../../aspose.cells.gridweb.data/rowfiltersettings/filterrows/)() | Фильтрует строки, используя строку критериев. |

### Примечания

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Этот класс будет удалён через 6 месяцев после августа 2014 г. Вы можете использовать GridWorksheet AddAutoFilter/FilterString для настроек автoфильтра/пользовательского фильтра. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

### См. также

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


