---
title: "Класс WebCells"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Aspose.Cells.GridWeb.Data.WebCells class."
type: docs
url: /ru/net/aspose.cells.gridweb.data/webcells/
---
## WebCells class

```csharp
[Obsolete("This class is obsolete; use  GridCells instead")]
public class WebCells
```

## Свойства

| Имя | Описание |
| --- | --- |
| [Count](../../aspose.cells.gridweb.data/webcells/count/) { get; } | Возвращает количество ячеек. |
| [Item](../../aspose.cells.gridweb.data/webcells/item/) { get; } | Получает элемент Cell по указанному индексу строки и индексу столбца ячейки. (2 индексатора) |
| [MaxColumn](../../aspose.cells.gridweb.data/webcells/maxcolumn/) { get; } |  |
| [MaxRow](../../aspose.cells.gridweb.data/webcells/maxrow/) { get; } |  |
| [MergedCells](../../aspose.cells.gridweb.data/webcells/mergedcells/) { get; } | Возвращает коллекцию объединённых ячеек. |
| [MinColumn](../../aspose.cells.gridweb.data/webcells/mincolumn/) { get; } | Минимальный номер столбца ячейки, содержащей данные или стиль. |
| [MinRow](../../aspose.cells.gridweb.data/webcells/minrow/) { get; } | Минимальный номер строки ячейки, содержащей данные или стиль. |
| [StandardHeight](../../aspose.cells.gridweb.data/webcells/standardheight/) { get; set; } | Возвращает или задает высоту строки по умолчанию в этом листе, в единицах точек. |
| [StandardWidth](../../aspose.cells.gridweb.data/webcells/standardwidth/) { get; set; } | Возвращает или задает ширину столбца по умолчанию в листе, в единицах символов. |

## Методы

| Имя | Описание |
| --- | --- |
| [Clear](../../aspose.cells.gridweb.data/webcells/clear/)() |  |
| [ClearContents](../../aspose.cells.gridweb.data/webcells/clearcontents/)(int, int, int, int) | Очищает содержимое диапазона. |
| [DeleteColumn](../../aspose.cells.gridweb.data/webcells/deletecolumn/)(int) | Удаляет столбец. |
| [DeleteRow](../../aspose.cells.gridweb.data/webcells/deleterow/)(int) | Удаляет строку. |
| [DeleteRows](../../aspose.cells.gridweb.data/webcells/deleterows/)(int, int) | Удаляет несколько строк. Этот метод гораздо быстрее, чем DeleteRow при пакетном удалении строк. |
| [Export](../../aspose.cells.gridweb.data/webcells/export/)(int, int, int, int, bool, bool) | Экспортирует данные из коллекции Cells веб‑листa WebWorksheet в новый объект DataTable |
| [ExportArray](../../aspose.cells.gridweb.data/webcells/exportarray/)(int, int, int, int) | Экспортирует данные из коллекции Cells в объект двумерного массива. |
| [GetColumnCaption](../../aspose.cells.gridweb.data/webcells/getcolumncaption/)(int) | Получает подпись столбца. Если подпись не задана, возвращает пустую строку. |
| [GetColumnReadonly](../../aspose.cells.gridweb.data/webcells/getcolumnreadonly/)(int) | Получает, является ли столбец только для чтения. Это расширенный метод GridWeb, который не сохраняется и не влияет на реальный файл Excel. |
| [GetColumnWidth](../../aspose.cells.gridweb.data/webcells/getcolumnwidth/)(int) | Возвращает ширину указанного столбца |
| [GetEnumerator](../../aspose.cells.gridweb.data/webcells/getenumerator/)() | Получает перечислитель ячеек |
| [GetRowCaption](../../aspose.cells.gridweb.data/webcells/getrowcaption/)(int) | Получает подпись строки. Если подпись не установлена, возвращает пустую строку. |
| [GetRowHeight](../../aspose.cells.gridweb.data/webcells/getrowheight/)(int) | Получает высоту указанной строки. |
| [GetRowHiddenStatus](../../aspose.cells.gridweb.data/webcells/getrowhiddenstatus/)(int) | Получить статус скрытия указанной строки. |
| [GetRowOutlineLevel](../../aspose.cells.gridweb.data/webcells/getrowoutlinelevel/)(int) | Получает уровень структуры строки. |
| [GetRowReadonly](../../aspose.cells.gridweb.data/webcells/getrowreadonly/)(int) | Получает, является ли строка только для чтения. Это расширенный метод GridWeb, он не сохраняется и не влияет на реальный файл Excel. |
| [InsertColumn](../../aspose.cells.gridweb.data/webcells/insertcolumn/)(int) | Вставляет новый столбец в лист. |
| [InsertRow](../../aspose.cells.gridweb.data/webcells/insertrow/)(int) | Вставляет новую строку в лист. |
| [InsertRows](../../aspose.cells.gridweb.data/webcells/insertrows/)(int, int) | Вставляет несколько строк в лист. |
| [Merge](../../aspose.cells.gridweb.data/webcells/merge/)(int, int, int, int) |  |
| [SetBorders](../../aspose.cells.gridweb.data/webcells/setborders/)(int, int, int, int, SetBorderPosition, WebBorderStyle) | Устанавливает границы для диапазона ячеек. |
| [SetColumnCaption](../../aspose.cells.gridweb.data/webcells/setcolumncaption/)(int, string) | Устанавливает подпись для столбца. Обратите внимание, что это расширенный атрибут и не сохраняется в файле Excel. |
| [SetColumnReadonly](../../aspose.cells.gridweb.data/webcells/setcolumnreadonly/)(int, bool) | Устанавливает столбец только для чтения, чтобы пользователь не мог удалить его на клиенте. Это расширенный метод GridWeb, он не сохраняется и не влияет на реальный файл Excel. |
| [SetColumnWidth](../../aspose.cells.gridweb.data/webcells/setcolumnwidth/)(int, Unit) | Устанавливает ширину указанного столбца. Принимаемый тип ширины: Point, Pixel или Inch. |
| [SetRowCaption](../../aspose.cells.gridweb.data/webcells/setrowcaption/)(int, string) | Устанавливает подпись для строки. |
| [SetRowHeight](../../aspose.cells.gridweb.data/webcells/setrowheight/)(int, Unit) | Устанавливает высоту указанной строки. Принимаемый тип ширины: Point, Pixel и Inch. |
| [SetRowHiddenStatus](../../aspose.cells.gridweb.data/webcells/setrowhiddenstatus/)(int, bool) | Установить статус скрытия указанной строки. |
| [SetRowOutlineLevel](../../aspose.cells.gridweb.data/webcells/setrowoutlinelevel/)(int, int) | Устанавливает уровень структуры строки. |
| [SetRowOutlineLevelAndStatus](../../aspose.cells.gridweb.data/webcells/setrowoutlinelevelandstatus/)(int, int, bool) | Устанавливает уровень структуры строки. |
| [SetRowReadonly](../../aspose.cells.gridweb.data/webcells/setrowreadonly/)(int, bool) | Устанавливает строку только для чтения, чтобы пользователь не мог удалить её на клиенте. Это расширенный метод GridWeb, он не сохраняется и не влияет на реальный файл Excel. |
| [SetStyle](../../aspose.cells.gridweb.data/webcells/setstyle/#setstyle_1)(string, TableItemStyle) | Устанавливает стиль для указанного диапазона ячеек. |
| [SetStyle](../../aspose.cells.gridweb.data/webcells/setstyle/#setstyle)(int, int, int, int, TableItemStyle) | Устанавливает стиль для указанного диапазона ячеек. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort)(int, int, int, int, int) | Сортирует данные по возрастанию сверху вниз в диапазоне WebWorksheet по указанному индексу столбца. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_2)(int, int, int, int, int[]) | Сортирует данные по возрастанию сверху вниз в диапазоне WebWorksheet по полям, указанным массивом индексов столбцов. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_1)(int, int, int, int, int, SortByOrder, SortOrientation, bool) | Сортирует данные по возрастанию сверху вниз в диапазоне WebWorksheet по указанному индексу столбца. |
| [Sort](../../aspose.cells.gridweb.data/webcells/sort/#sort_3)(int, int, int, int, int[], SortByOrder[], SortOrientation, bool) | Сортирует данные по возрастанию в диапазоне WebWorksheet по полям, указанным массивом индексов. |
| [UnMerge](../../aspose.cells.gridweb.data/webcells/unmerge/)(int, int, int, int) | Разъединяет указанный диапазон объединённых ячеек. |
| static [CellIndexToName](../../aspose.cells.gridweb.data/webcells/cellindextoname/)(int, int) | Получает имя ячейки в соответствии с её индексами строки и столбца. |
| static [CellNameToIndex](../../aspose.cells.gridweb.data/webcells/cellnametoindex/)(string, out int, out int) | Получает индексы строки и столбца ячейки по её имени |
| static [ColumnIndexToName](../../aspose.cells.gridweb.data/webcells/columnindextoname/)(int) | Получает имя столбца в соответствии с индексом столбца. |
| static [ColumnNameToIndex](../../aspose.cells.gridweb.data/webcells/columnnametoindex/)(string) | Получает индекс столбца в соответствии с именем столбца. |

### Примечания

ПРИМЕЧАНИЕ: Этот класс теперь устарел. Пожалуйста, используйте GridCells вместо него. Этот класс будет удалён через 6 месяцев после августа 2014 г. Aspose извиняется за любые причинённые неудобства.

### См. также

* namespace [Aspose.Cells.GridWeb.Data](../../aspose.cells.gridweb.data/)
* assembly [Aspose.Cells.GridWeb](../../)


