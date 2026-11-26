---
title: "Класс Range"
second_title: "Справочник API Aspose.Cells для .NET"
description: "Класс Aspose.Cells.Range. Инкапсулирует объект, представляющий диапазон ячеек в электронной таблице"
type: docs
url: /ru/net/aspose.cells/range/
---
## Range class

Инкапсулирует объект, представляющий диапазон ячеек в электронной таблице.

```csharp
public class Range : IEnumerable
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Range](range/#constructor)(CellArea, Cells) | Конструктор класса. |
| [Range](range/#constructor_1)(int, int, int, int, Cells) | Конструктор класса. |

## Свойства

| Имя | Описание |
| --- | --- |
| [Address](../../aspose.cells/range/address/) { get; } | Получает адрес диапазона. |
| [ColumnCount](../../aspose.cells/range/columncount/) { get; } | Получает количество столбцов в диапазоне. |
| [ColumnWidth](../../aspose.cells/range/columnwidth/) { get; set; } | Устанавливает или получает ширину столбца этого диапазона. |
| [CurrentRegion](../../aspose.cells/range/currentregion/) { get; } | Возвращает объект Range, представляющий текущий регион. Текущий регион — это диапазон, ограниченный любой комбинацией пустых строк и пустых столбцов. |
| [EntireColumn](../../aspose.cells/range/entirecolumn/) { get; } | Получает объект Range, представляющий весь столбец (или столбцы), содержащий указанный диапазон. |
| [EntireRow](../../aspose.cells/range/entirerow/) { get; } | Получает объект Range, представляющий всю строку (или строки), содержащую указанный диапазон. |
| [FirstColumn](../../aspose.cells/range/firstcolumn/) { get; } | Получает индекс первого столбца диапазона. |
| [FirstRow](../../aspose.cells/range/firstrow/) { get; } | Получает индекс первой строки диапазона. |
| [Height](../../aspose.cells/range/height/) { get; } | Получает ширину диапазона в пунктах. |
| [Hyperlinks](../../aspose.cells/range/hyperlinks/) { get; } | Получает все гиперссылки в диапазоне. |
| [Item](../../aspose.cells/range/item/) { get; } | Получает объект [`Cell`](../cell/) в этом диапазоне. |
| [Left](../../aspose.cells/range/left/) { get; } | Получает расстояние в пунктах от левого края столбца A до левого края диапазона. |
| [Name](../../aspose.cells/range/name/) { get; set; } | Получает или задает имя диапазона. |
| [RefersTo](../../aspose.cells/range/refersto/) { get; } | Получает значение свойства RefersTo диапазона. |
| [RowCount](../../aspose.cells/range/rowcount/) { get; } | Получает количество строк в диапазоне. |
| [RowHeight](../../aspose.cells/range/rowheight/) { get; set; } | Устанавливает или получает высоту строк в этом диапазоне |
| [Top](../../aspose.cells/range/top/) { get; } | Получает расстояние в пунктах от верхнего края строки 1 до верхнего края диапазона. |
| [Value](../../aspose.cells/range/value/) { get; set; } | Получает и задает значение диапазона. |
| [Width](../../aspose.cells/range/width/) { get; } | Получает ширину диапазона в пунктах. |
| [Worksheet](../../aspose.cells/range/worksheet/) { get; } | Получает объект [`Worksheet`](./worksheet/), который содержит этот диапазон. |

## Методы

| Имя | Описание |
| --- | --- |
| [AddHyperlink](../../aspose.cells/range/addhyperlink/)(string, string, string) | Добавляет гиперссылку в указанную ячейку или диапазон ячеек. |
| [ApplyStyle](../../aspose.cells/range/applystyle/)(Style, StyleFlag) | Применяет форматы ко всему диапазону. |
| [AutoFill](../../aspose.cells/range/autofill/#autofill)(Range) | Автоматически заполняет целевой диапазон. |
| [AutoFill](../../aspose.cells/range/autofill/#autofill_1)(Range, AutoFillType) | Автоматически заполняет целевой диапазон. |
| [Clear](../../aspose.cells/range/clear/)() | Очищает этот диапазон. |
| [ClearComments](../../aspose.cells/range/clearcomments/)() | Очищает комментарии этого диапазона. |
| [ClearContents](../../aspose.cells/range/clearcontents/)() | Очищает содержимое этого диапазона. |
| [ClearFormats](../../aspose.cells/range/clearformats/)() | Очищает форматы этого диапазона. |
| [ClearHyperlinks](../../aspose.cells/range/clearhyperlinks/)(bool) | Только удаляет гиперссылки. |
| [Copy](../../aspose.cells/range/copy/#copy)(Range) | Копирует данные (включая формулы), форматирование, графические объекты и т.д. из исходного диапазона. |
| [Copy](../../aspose.cells/range/copy/#copy_1)(Range, PasteOptions) | Копирует диапазон с параметрами специальной вставки. |
| [CopyData](../../aspose.cells/range/copydata/)(Range) | Копирует данные ячейки (включая формулы) из исходного диапазона. |
| [CopyStyle](../../aspose.cells/range/copystyle/)(Range) | Копирует настройки стиля из исходного диапазона. |
| [CopyValue](../../aspose.cells/range/copyvalue/)(Range) | Копирует значение ячейки из исходного диапазона. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable/#exportdatatable)() | Экспортирует данные из этого диапазона в объект DataTable. |
| [ExportDataTable](../../aspose.cells/range/exportdatatable/#exportdatatable_1)(ExportTableOptions) | Экспортирует данные из этого диапазона в объект DataTable. |
| [ExportDataTableAsString](../../aspose.cells/range/exportdatatableasstring/)() | Экспортирует данные из этого диапазона в объект DataTable. |
| [GetCellOrNull](../../aspose.cells/range/getcellornull/)(int, int) | Получает объект [`Cell`](../cell/) или null в этом диапазоне. |
| [GetEnumerator](../../aspose.cells/range/getenumerator/)() | Получает перечислитель для ячеек в этом Range. |
| [GetOffset](../../aspose.cells/range/getoffset/)(int, int) | Получает диапазон `Range` со смещением. |
| [Intersect](../../aspose.cells/range/intersect/)(Range) | Возвращает объект `Range`, представляющий прямоугольное пересечение двух диапазонов. |
| [IsBlank](../../aspose.cells/range/isblank/)() | Указывает, содержит ли диапазон значения. |
| [IsIntersect](../../aspose.cells/range/isintersect/)(Range) | Указывает, пересекается ли диапазон. |
| [Merge](../../aspose.cells/range/merge/)() | Объединяет диапазон ячеек в одну ячейку. |
| [MoveTo](../../aspose.cells/range/moveto/)(int, int) | Перемещает текущий диапазон в целевой диапазон. |
| [PutValue](../../aspose.cells/range/putvalue/)(string, bool, bool) | Помещает значение в диапазон; при необходимости значение будет преобразовано в другой тип данных, а числовой формат ячейки будет сброшен. |
| [SetInsideBorders](../../aspose.cells/range/setinsideborders/)(BorderType, CellBorderType, CellsColor) | Устанавливает внутренние границы диапазона. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder/#setoutlineborder)(BorderType, CellBorderType, CellsColor) | Устанавливает контурную границу вокруг диапазона ячеек. |
| [SetOutlineBorder](../../aspose.cells/range/setoutlineborder/#setoutlineborder_1)(BorderType, CellBorderType, Color) | Устанавливает контурную границу вокруг диапазона ячеек. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders)(CellBorderType, CellsColor) | Устанавливает контурные границы вокруг диапазона ячеек с одинаковым стилем и цветом границы. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders_1)(CellBorderType, Color) | Устанавливает контурные границы вокруг диапазона ячеек с одинаковым стилем и цветом границы. |
| [SetOutlineBorders](../../aspose.cells/range/setoutlineborders/#setoutlineborders_2)(CellBorderType[], Color[]) | Устанавливает внешние границы вокруг диапазона ячеек. |
| [SetStyle](../../aspose.cells/range/setstyle/#setstyle)(Style) | Устанавливает стиль диапазона. |
| [SetStyle](../../aspose.cells/range/setstyle/#setstyle_1)(Style, bool) | Применить стиль ячейки. |
| [ToHtml](../../aspose.cells/range/tohtml/)(HtmlSaveOptions) | Преобразовать диапазон в html . |
| [ToImage](../../aspose.cells/range/toimage/)(ImageOrPrintOptions) | Преобразует диапазон в изображение. |
| [ToJson](../../aspose.cells/range/tojson/)(JsonSaveOptions) | Преобразовать диапазон в значение JSON. |
| override [ToString](../../aspose.cells/range/tostring/)() | Возвращает строку, представляющую текущий объект Range. |
| [Transpose](../../aspose.cells/range/transpose/)() | Транспонировать (повернуть) данные из строк в столбцы или наоборот. |
| [Union](../../aspose.cells/range/union/)(Range) | (**Obsolete.**) Возвращает объединение двух диапазонов. |
| [UnionRang](../../aspose.cells/range/unionrang/)(Range) | (**Obsolete.**) Возвращает результат объединения двух диапазонов. |
| [UnionRanges](../../aspose.cells/range/unionranges/)(Range[]) | Возвращает результат объединения двух диапазонов. |
| [UnMerge](../../aspose.cells/range/unmerge/)() | Разъединяет объединённые ячейки этого диапазона. |

### Примечания

Класс Range обозначает область электронных таблиц Excel. С его помощью вы можете форматировать и задавать значение диапазона. И вы также можете просто копировать диапазон Excel.

### Примеры

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassRangeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            Aspose.Cells.Range range = cells.CreateRange("A1", "D3");
            range.Value = "Hello";
            workbook.Save("book1.xlsm");
        }
    }
}
```

### См. также

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


