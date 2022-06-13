---
title: Range
second_title: Справочник по Aspose.Cells для .NET API
description: Инкапсулирует объект представляющий диапазон ячеек в электронной таблице.
type: docs
weight: 5030
url: /ru/net/aspose.cells/range/
---
## Range class

Инкапсулирует объект, представляющий диапазон ячеек в электронной таблице.

```csharp
public class Range
```

## Характеристики

| Имя | Описание |
| --- | --- |
| [Address](../../aspose.cells/range/address) { get; } | Получает адрес диапазона. |
| [ColumnCount](../../aspose.cells/range/columncount) { get; } | Получает количество столбцов в диапазоне. |
| [ColumnWidth](../../aspose.cells/range/columnwidth) { get; set; } | Устанавливает или получает ширину столбца этого диапазона |
| [CurrentRegion](../../aspose.cells/range/currentregion) { get; } | Возвращает объект Range, представляющий текущий регион. Текущая область представляет собой диапазон, ограниченный любой комбинацией пустых строк и пустых столбцов. |
| [EntireColumn](../../aspose.cells/range/entirecolumn) { get; } | Получает объект Range, представляющий весь столбец (или столбцы), содержащий указанный диапазон. |
| [EntireRow](../../aspose.cells/range/entirerow) { get; } | Получает объект Range, представляющий всю строку (или строки), содержащие указанный диапазон. |
| [FirstColumn](../../aspose.cells/range/firstcolumn) { get; } | Получает индекс первого столбца диапазона. |
| [FirstRow](../../aspose.cells/range/firstrow) { get; } | Получает индекс первой строки диапазона. |
| [Hyperlinks](../../aspose.cells/range/hyperlinks) { get; } | Получает все гиперссылки в диапазоне. |
| [Item](../../aspose.cells/range/item) { get; } | Получает[`Cell`](../cell)объект в этом диапазоне. |
| [Name](../../aspose.cells/range/name) { get; set; } | Получает или задает имя диапазона. |
| [RefersTo](../../aspose.cells/range/refersto) { get; } | Получает ссылки на диапазон. |
| [RowCount](../../aspose.cells/range/rowcount) { get; } | Получает количество строк в диапазоне. |
| [RowHeight](../../aspose.cells/range/rowheight) { get; set; } | Устанавливает или получает высоту строк в этом диапазоне |
| [Value](../../aspose.cells/range/value) { get; set; } | Получает и устанавливает значение диапазона. |
| [Worksheet](../../aspose.cells/range/worksheet) { get; } | Получает объект[`Worksheet`](./worksheet), содержащий этот диапазон. |

## Методы

| Имя | Описание |
| --- | --- |
| [ApplyStyle](../../aspose.cells/range/applystyle)(Style, StyleFlag) | Применяет форматы ко всему диапазону. |
| [AutoFill](../../aspose.cells/range/autofill#autofill)(Range) | Автоматически заполняет целевой диапазон. |
| [AutoFill](../../aspose.cells/range/autofill#autofill_1)(Range, AutoFillType) | Автоматически заполняет целевой диапазон. |
| [Copy](../../aspose.cells/range/copy#copy)(Range) | Копирует данные (включая формулы), форматирование, объекты рисования и т. д. из исходного диапазона. |
| [Copy](../../aspose.cells/range/copy#copy_1)(Range, PasteOptions) | Копирование диапазона со специальными параметрами вставки. |
| [CopyData](../../aspose.cells/range/copydata)(Range) | Копирует данные ячейки (включая формулы) из исходного диапазона. |
| [CopyStyle](../../aspose.cells/range/copystyle)(Range) | Копирует настройки стиля из исходного диапазона. |
| [CopyValue](../../aspose.cells/range/copyvalue)(Range) | Копирует значение ячейки из исходного диапазона. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable)() | Экспортирует данные из этого диапазона в объектDataTable. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable#exportdatatable_1)(ExportTableOptions) | Экспортирует данные из этого диапазона в объектDataTable. |
| [ExportDataTableAsString](../../aspose.cells/range/exportdatatableasstring)() | Экспортирует данные из этого диапазона в объектDataTable. |
| [GetCellOrNull](../../aspose.cells/range/getcellornull)(int, int) | Получает объект[`Cell`](../cell)или null в этом диапазоне. |
| [GetEnumerator](../../aspose.cells/range/getenumerator)() | Получает перечислитель для ячеек в этом диапазоне. |
| [GetOffset](../../aspose.cells/range/getoffset)(int, int) | Получает[`Range`](../range)диапазон по смещению. |
| [Intersect](../../aspose.cells/range/intersect)(Range) | Возвращает объект[`Range`](../range), представляющий прямоугольное пересечение двух диапазонов. |
| [IsIntersect](../../aspose.cells/range/isintersect)(Range) | Указывает, пересекается ли диапазон. |
| [Merge](../../aspose.cells/range/merge)() | Объединяет диапазон ячеек в одну ячейку. |
| [MoveTo](../../aspose.cells/range/moveto)(int, int) | Переместить текущий диапазон в целевой диапазон. |
| [PutValue](../../aspose.cells/range/putvalue)(string, bool, bool) | Помещает значение в диапазон, при необходимости значение будет преобразовано в другой тип данных, а формат номера ячейки будет сброшен. |
| [SetInsideBorders](../../aspose.cells/range/setinsideborders)(BorderType, CellBorderType, CellsColor) | Установить внутренние границы диапазона. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder)(BorderType, CellBorderType, Color) | Устанавливает границу контура вокруг диапазона ячеек. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders)(CellBorderType, Color) | Устанавливает границы контура вокруг диапазона ячеек с одинаковым стилем и цветом границы. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders#setoutlineborders_1)(CellBorderType[], Color[]) | Устанавливает границы строки вокруг диапазона ячеек. |
| [SetStyle](../../aspose.cells/range/setstyle)(Style) | Устанавливает стиль диапазона. |
| override [ToString](../../aspose.cells/range/tostring)() | Возвращает строку, представляющую текущий объект Range. |
| [Union](../../aspose.cells/range/union)(Range) | Возвращает объединение двух диапазонов. |
| [UnMerge](../../aspose.cells/range/unmerge)() | Разъединяет объединенные ячейки этого диапазона. |

### Примеры

```csharp

[C#]

  //Создание экземпляра рабочей книги object
Workbook workbook = new Workbook();
// Получить первые ячейки рабочего листа.
Cells cells = workbook.Worksheets[0].Cells;
  // Создаем диапазон (A1:D3).
Range range = cells.CreateRange("A1", "D3");
  // Установить значение в диапазоне.
range.Value = "Hello";
  // Сохраняем файл Excel
workbook.Save("book1.xlsm");

 [Visual Basic]

'Instantiating a Workbook object
Dim workbook As Workbook = New Workbook()
'Get the first Worksheet Cells.
Dim cells as Cells = workbook.Worksheets[0].Cells
'Create a range (A1:D3).
Dim range as Range = cells.CreateRange("A1", "D3")
'Set value to the range.
range.Value = "Hello"
'Save the Excel file
workbook.Save("book1.xlsm")
```

### Смотрите также

* пространство имен [Aspose.Cells](../../aspose.cells)
* сборка [Aspose.Cells](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
